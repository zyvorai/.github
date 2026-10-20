# AI code review (zyvor-org-profile)

_Generated 2026-10-20 by claude-opus-5-5 from a snapshot of tracked sources; verify before acting._

# Code review: zyvor-org-profile

## Summary

This repo holds the GitHub organization profile for **@zyvorai**. It contains:

- `profile/README.md`, the content to publish to `zyvorai/.github`.
- Three operator runbooks: `SETUP.md`, `GITHUB_ORG_SETTINGS.md` and `LEADS.md`.
- A top-level `README.md` explaining how to publish.

There is no code. The content is marketing Markdown/HTML plus manual org-configuration and lead-tracking instructions.

## Bugs and correctness risks

**The runbooks contradict each other and the profile.**

- **Verify checklist vs. profile:** `GITHUB_ORG_SETTINGS.md` says the profile should show "Axiom + Edge Stack + current Community Edition repos (no Aether)". `profile/README.md` does the opposite:
  - It never mentions Axiom.
  - It does link Aether (`github.com/zyvorai/Aether`) in the "All open-source projects" table.
- **Pinned repos:**
  - `GITHUB_ORG_SETTINGS.md` pins `guestkit, fabric, kryton, haven, scout, edge-stack`.
  - `SETUP.md` pins `guestkit, fabric, kryton, haven, scout, kairo`.
- **Bio:** The two files specify different bios. `SETUP.md` includes "KubeVirt", while the profile positions Kairon as "no virt-launcher". That is a messaging conflict, not a functional bug.

**Repository names drift across files.**

- `SETUP.md` refers to `zyvorai/guestkit`, `zyvorai/fabric` and `zyvorai/kryton`.
- The profile links `zyvor-guestkit`, `zyvorai-fabric` and `zyvor-kryton`.
- `LEADS.md` uses `hyper2kvm`, while the profile uses `zyvor-h2kvm`.
- Naming mixes three conventions: `zyvor-*`, `zyvorai-*` and bare names (`nodra`, `scout`, `janus`).
- At least one set of these names is likely stale. Pins may fail or rely on rename redirects.
- I can't verify which repos actually exist.

**Publish steps may not ship the images.**

- `profile/README.md` hot-links many assets: `profile/assets/hero-*.svg`, `cards/*.svg`, `terminal.svg` and `stack.svg`.
- The publish snippet in `README.md` only runs `git add profile/README.md`.
- No `profile/assets/` files appear in this snapshot. This may be truncation, but if the assets are absent, every hero, card and diagram image is broken.

**The publish snippet assumes the wrong directory.** It runs `cd zyvorai-github`, but this repo is `zyvor-org-profile`.

**Image URLs are fragile.**

- They are hard-coded to the `main` branch of `zyvorai/.github`.
- They use a manual cache-buster, `?v=blue1`. Nothing documents that this value must be bumped when assets change, so stale images are likely after edits.

**The "Try it in 60 seconds" commands are not self-contained.**

- `examples/qemu.json` is a relative path that only resolves inside a FluxVM checkout.
- `ubuntu.qcow2` is assumed to exist locally.
- No install step is given for `fluxctl` or `kaironctl`.
- `fluxctl create` runs under `sudo` but `fluxctl exec` does not. This may hit permission or socket mismatches; I can't verify how the CLI behaves.

**The `#try-it` anchor may not work.** It relies on `<a id="try-it">`. GitHub rewrites ids to `user-content-*` and depends on JavaScript to resolve the hash. This should be verified on the rendered page.

**Minor issues in `profile/README.md`:**

- The "Talk to us" badge uses `logo=maildotru`, which is the Mail.Ru brand logo and probably not intended.
- The Kairon and GuestKit "quick start" links lack the `#quick-start` anchor that the FluxVM link has.
- Edge Stack links to Pages in the card but to the repo in the table.

**Inconsistent URL pattern in `SETUP.md`:** the About-box table uses `zyvor.dev/zyvor-fabric` while every other entry uses `zyvor.dev/<short-name>`.

## Security concerns

- **Personal email for recruiting:** "Join us" publishes `zyvorailabs@gmail.com`, a consumer Gmail address. This weakens trust, makes impersonation and phishing easier, and puts candidate data in a personal account. Use a domain address such as `jobs@zyvor.dev`.
- **Spam exposure:** `sales@zyvor.dev` is published in several places. That is expected, but it should have spam filtering in place.
- **Privacy and consent:** `LEADS.md` describes capturing `utm_*` in hidden form fields "when visitor accepted cookies", plus GA/Plausible and a `POST /api/v1/track` endpoint.
  - Nothing here covers consent handling, data retention, or whether `/api/v1/track` is authenticated or rate-limited.
  - These live in other repos (`hypersdk-web`), so this can't be verified here, but it is worth a review.
- **Running privileged commands:** the quick start tells users to run `sudo fluxctl` against a spec file without saying where to get it or how to verify the binary. Consider linking to signed releases; `zysign` is listed as an org tool.
- **No license file:** the profile advertises "Apache-2.0 at the core", but this repo itself has no visible LICENSE file. This is low risk for a profile repo, but it is inconsistent.

## Test and CI gaps

- There is no CI at all. Useful additions:
  - **Link checking** (e.g. lychee or markdown-link-check) over `profile/README.md` and the docs. Roughly 60 external repo, Pages and asset links are prone to rot, especially given the naming drift.
  - **Asset existence check:** every `raw.githubusercontent.com/.../profile/assets/...` reference should map to a file in the repo.
  - **markdownlint or HTML validation** for the embedded HTML tables.
  - **Consistency check:** a single source of truth (e.g. a YAML file listing repos, pins and bio) with a script or CI step that diffs it against `SETUP.md`, `GITHUB_ORG_SETTINGS.md` and the profile.
- There is no automated publish step. The workflow is manual `git push` per `README.md`, and nothing confirms whether this repo *is* `zyvorai/.github` or a staging copy.

## Documentation gaps

- **No authoritative runbook:** `SETUP.md` and `GITHUB_ORG_SETTINGS.md` overlap and conflict, and neither is marked authoritative.
- **Unclear conversion status:**
  - `SETUP.md` treats conversion to an organization as still pending ("Until then, the user profile README is zyvorai/zyvorai").
  - The profile already assumes `zyvorai/.github` is live.
- **No asset docs:** nothing explains how the `profile/assets` SVGs are produced or edited, or the `?v=` cache-bust convention.
- **Vague comment:** the comment `<!-- utm: github / zyvorai_org (in href only) -->` hints at the convention in `LEADS.md` without referencing it.
- **Missing context and repo hygiene:**
  - `README.md` mentions `hypersdk`, but the profile never links it, and its relationship to FluxVM and the other projects is unexplained.
  - No CONTRIBUTING or ownership notes say who may edit the profile or settings.
- **Unverifiable reference:** `LEADS.md` points at `src/utils/marketingAttribution.ts` in another repo. I can't verify that path.

## Top 5 recommended actions

1. **Reconcile repo names everywhere.** Settle on actual repo slugs and fix `SETUP.md`, `GITHUB_ORG_SETTINGS.md`, `LEADS.md` and `profile/README.md`. Resolve the Aether/Axiom contradiction and the pin list (`edge-stack` vs `kairo`).
2. **Merge the runbooks.** Combine `SETUP.md` and `GITHUB_ORG_SETTINGS.md` into one authoritative runbook, with one bio and one pin list.
3. **Ensure assets are committed and published.** Change the publish snippet to `git add profile/` and fix the `cd` path. Document or automate the `?v=` cache-bust.
4. **Add CI.** Include a link checker, an asset-existence check and markdownlint, optionally driven from a single repo-list data file.
5. **Fix the contact and quick-start content:**
   - Replace the Gmail recruiting address with a domain address.
   - Make the quick start self-contained (install step, where the spec and image come from, consistent `sudo` use).
   - Verify the `#try-it` anchor and the `maildotru` badge logo.
