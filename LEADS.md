# Measuring GitHub → Zyvor leads

## UTM convention

All GitHub README and issue-template links should use:

`utm_source=github&utm_medium=<repo>`

Examples: `hyper2kvm`, `hypersdk`, `guestkit`, `netevd`, `netctl`, `cloud-netconfig`, `zyvorai_org` (org profile).

Package tarballs use `utm_source=package&utm_medium=<product>`.

## Where leads are captured

| Channel | What to check |
|---------|----------------|
| **zyvor.dev/contact** | Form submissions; hidden fields include `utm_*` when visitor accepted cookies |
| **sales@zyvor.dev** | Direct email from issue templates and README |
| **Plausible / GA** | Referrers from `github.com` (set `PLAUSIBLE_DOMAIN` / `GA_MEASUREMENT_ID` on website build) |
| **Dashboard API** | `POST /api/v1/track` events include attribution properties |

## Monthly review

1. Contact form exports: group by `utm_medium`
2. Top referrers in analytics: `github.com/zyvorai/*`
3. Double down on README/issue links for repos that convert

## Website

Source: [zyvorai/hypersdk-web](https://github.com/zyvorai/hypersdk-web) (Docusaurus site for zyvor.dev). Referrer-based attribution is implemented in `src/utils/marketingAttribution.ts`.
