<!-- utm: github / zyvorai_org (in href only) -->

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zyvorai/.github/main/profile/assets/github-banner.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zyvorai/.github/main/profile/assets/github-banner-light.svg">
    <img src="https://raw.githubusercontent.com/zyvorai/.github/main/profile/assets/github-banner.svg" alt="Zyvor — open infrastructure for migration, Kubernetes, and the edge" width="100%">
  </picture>
</p>

<h3 align="center">Enterprise infrastructure for the post-legacy estate</h3>
<p align="center">
  Migrate off proprietary hypervisors &amp; HCI platforms, run on Kubernetes &amp; KubeVirt, operate a private cloud with <b>Axiom</b> —
  one API contract across every layer.<br/>
  <sub><a href="https://zyvor.dev?utm_source=github&utm_medium=zyvorai_org">Zyvor</a> · zyvor.dev</sub>
</p>

<p align="center">
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/▶_Watch_demo-cc420a?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch demo"/></a>
  <a href="https://zyvor.dev/axiom?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Axiom-private_cloud-1f2937?style=for-the-badge" alt="Axiom"/></a>
  <a href="https://zyvor.dev/contact?intent=demo&utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Book_engineering_call-16a34a?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book call"/></a>
  <a href="mailto:sales@zyvor.dev"><img src="https://img.shields.io/badge/sales%40zyvor.dev-2563eb?style=for-the-badge&logo=gmail&logoColor=white" alt="Sales"/></a>
</p>

<p align="center">
  <a href="https://github.com/zyvorai/transiva/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/transiva?style=flat-square&logo=github&label=transiva&labelColor=18181B&color=cc420a" alt="transiva"/></a>
  <a href="https://github.com/zyvorai/guestkit/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/guestkit?style=flat-square&logo=github&label=guestkit&labelColor=18181B&color=cc420a" alt="guestkit"/></a>
  <a href="https://github.com/zyvorai/haven/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/haven?style=flat-square&logo=github&label=haven&labelColor=18181B&color=cc420a" alt="haven"/></a>
  <a href="https://github.com/zyvorai/kairon/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/kairon?style=flat-square&logo=github&label=kairon&labelColor=18181B&color=cc420a" alt="kairon"/></a>
  <a href="https://github.com/zyvorai/edge-stack/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/edge-stack?style=flat-square&logo=github&label=edge-stack&labelColor=18181B&color=cc420a" alt="edge-stack"/></a>
  <a href="https://github.com/zyvorai/yard/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/yard?style=flat-square&logo=github&label=yard&labelColor=18181B&color=cc420a" alt="yard"/></a>
  <a href="https://github.com/zyvorai/gryvia/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/gryvia?style=flat-square&logo=github&label=gryvia&labelColor=18181B&color=cc420a" alt="gryvia"/></a>
  <a href="https://github.com/zyvorai/zyntra/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/zyntra?style=flat-square&logo=github&label=zyntra&labelColor=18181B&color=cc420a" alt="zyntra"/></a>
  <img src="https://img.shields.io/badge/Apache--2.0-community-18181B?style=flat-square&labelColor=18181B" alt="Apache-2.0"/>
</p>

---

## Try it in 60 seconds

```bash
# Community Edition preview — export, convert, and validate a VM offline
$ transivactl export --provider enterprise-hypervisor --vm prod-db-01 --target kvm
→ Discovered (4 vCPU · 32 GiB · 420 GB)       ✓
→ Streamed export with integrity checks       ✓
→ h2kvm: QCOW2 + VirtIO + bootloader          ✓
→ GuestKit: guest validated offline           ✓
→ First boot on KVM                           ✓  6.8s

# Fleet migrations, SLAs, air-gapped rollouts → talk to Zyvor
```

<p align="center">
  <b>See the real platform first</b> — migration video, Axiom private cloud, an optional 30-minute engineering session<br/>
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org"><b>Demo</b></a>
  ·
  <a href="https://zyvor.dev/axiom?utm_source=github&utm_medium=zyvorai_org"><b>Axiom</b></a>
  ·
  <a href="https://zyvor.dev/contact?utm_source=github&utm_medium=zyvorai_org"><b>Contact</b></a>
</p>

---

## Edge Stack — how the edge products work together

Hardware discovery → offline runtime → fleet control → signed OS updates → ops console → Relay event loop.

| | |
|:---|:---|
| **Landing + suite CI** | [zyvorai.github.io/edge-stack](https://zyvorai.github.io/edge-stack/) · [suite CI](https://github.com/zyvorai/edge-stack/actions/workflows/suite-ci.yml) |
| **How they fit** | [docs/HOW_THEY_FIT.md](https://github.com/zyvorai/edge-stack/blob/main/docs/HOW_THEY_FIT.md) |
| **Products** | [Device Agent](https://github.com/zyvorai/device-agent) · [Nodra](https://github.com/zyvorai/nodra) · [Fleet](https://github.com/zyvorai/fleet) · [OTA](https://github.com/zyvorai/ota) · [Yard](https://github.com/zyvorai/yard) · [relay-edge](https://github.com/zyvorai/relay-edge) · [relay-pubsub](https://github.com/zyvorai/relay-pubsub) |

Hermetic **suite-ci** proves Device Agent → Yard, Nodra → Yard, Fleet → Yard, and relay-pubsub backend contracts on every push — without claiming each product’s full qualify matrix.

---

## Sovereign AI OS — GPUs, decisions, and the network on your own hardware

Gryvia schedules the GPUs → Zyntra turns live signals into ranked, human-approved actions → Netra watches and enforces the network. Agents can propose; only people approve, and every action lands in a signed audit.

| | |
|:---|:---|
| **Products** | [Gryvia](https://github.com/zyvorai/gryvia) — GPU-aware scheduling, GPU as a Service, models and inference · [Zyntra](https://github.com/zyvorai/zyntra) — decision intelligence: sense, simulate, act · [Netra](https://github.com/zyvorai/netra) — eBPF observability and emergency network control |
| **How they fit** | [docs/sovereign-aios.md](https://github.com/zyvorai/gryvia/blob/main/docs/sovereign-aios.md) · [Gryvia docs](https://zyvorai.github.io/gryvia/) |
| **Status** | Alpha. Runs on Kubernetes (k3s and up); air-gap ready. |

---

## What makes this different

<table>
<tr>
<td width="33%" align="center" valign="top">

### One pipeline
Not a stack of point tools. **Export → convert → fix → deploy → operate**, one suite, one API contract.

</td>
<td width="33%" align="center" valign="top">

### Private cloud on k8s
**Axiom** is the day-2 console (k3s → production). **Ragnarok** attests confidential / disposable VMs.

</td>
<td width="33%" align="center" valign="top">

### Enterprise-ready
RBAC/SSO, audit logs, **air-gapped** deployment — built for regulated industries from day one.

</td>
</tr>
</table>

---

## The suite, by what it does to your estate

| Category | What it covers | Explore |
|:---|:---|:---|
| **Migrate** | Discover, simulate, convert, and assure workloads off proprietary hypervisors, HCI, and public cloud | [Transiva](https://zyvor.dev/transiva?utm_source=github&utm_medium=zyvorai_org) · [Scout](https://zyvor.dev/scout?utm_source=github&utm_medium=zyvorai_org) · [Chimera](https://zyvor.dev/chimera?utm_source=github&utm_medium=zyvorai_org) · [h2kvm](https://zyvor.dev/h2kvm?utm_source=github&utm_medium=zyvorai_org) · [GuestKit](https://zyvor.dev/guestkit?utm_source=github&utm_medium=zyvorai_org) |
| **Run** | Operate VMs and apps on Kubernetes, KubeVirt, and libvirt from one control plane | [Kairon](https://zyvor.dev?utm_source=github&utm_medium=zyvorai_org) · [Zorvia](https://github.com/zyvorai/zorvia) · [Kryton](https://zyvor.dev/kryton?utm_source=github&utm_medium=zyvorai_org) · [Haven](https://zyvor.dev/haven?utm_source=github&utm_medium=zyvorai_org) · [Fabric](https://zyvor.dev/zyvor-fabric?utm_source=github&utm_medium=zyvorai_org) · [FluxVM](https://zyvor.dev/fluxvm?utm_source=github&utm_medium=zyvorai_org) · [Fleet](https://github.com/zyvorai/fleet) |
| **Operate** | Private cloud day-2, storage, packets, GPUs, network, reliability | [Axiom](https://zyvor.dev/axiom?utm_source=github&utm_medium=zyvorai_org) · [Atlas](https://github.com/zyvorai/atlas) · [Ragnarok](https://zyvor.dev/ragnarok?utm_source=github&utm_medium=zyvorai_org) · [PacketWolf](https://zyvor.dev/packetwolf?utm_source=github&utm_medium=zyvorai_org) · [Zynera](https://github.com/zyvorai/zynera) · [Netra](https://zyvorai.github.io/netra/) · [Paqtra](https://zyvorai.github.io/paqtra/) · [Rivora](https://zyvorai.github.io/rivora/) · [Shukra](https://github.com/zyvorai/shukra) · [Duvora](https://github.com/zyvorai/duvora) · [Yard](https://zyvorai.github.io/yard/) |
| **AI** | Schedule GPUs, serve models, and turn live signals into human-approved actions — the Sovereign AI OS | [Gryvia](https://zyvorai.github.io/gryvia/) · [Zyntra](https://github.com/zyvorai/zyntra) · [Solvor](https://github.com/zyvorai/solvor) |
| **Scale** | Stand up clusters, sign documents, edge OTA | [HyperCluster](https://github.com/zyvorai/hypercluster) · [ZySign](https://github.com/zyvorai/zysign) · [OTA](https://zyvorai.github.io/ota/) |
| **Edge** | Next: how Device Agent → Nodra → Fleet → OTA → Yard → Relay fit as one stack | **[Edge Stack →](https://zyvorai.github.io/edge-stack/)** |
| **Community Edition** | Apache-2.0 tools in this org — source + GitHub Pages | ↓ table below |

<p align="center"><a href="https://zyvor.dev/products?utm_source=github&utm_medium=zyvorai_org">Full product catalogue →</a> · <a href="https://zyvor.dev/compare?utm_source=github&utm_medium=zyvorai_org">Compare all products →</a> · <a href="https://zyvorai.github.io/edge-stack/">Edge Stack (how they fit) →</a></p>

---

## Open source vs Enterprise

Everything below is real, working, Apache-2.0 source — not a crippled trial. Enterprise is support, scale programs, and hardened deployments on top of it, not features withheld from the repo.

| | Open source (these repos) | Enterprise ([zyvor.dev](https://zyvor.dev?utm_source=github&utm_medium=zyvorai_org)) |
|:---|:---|:---|
| **Good for** | Labs, CI gates, single-VM / small-fleet migrations, contributing | Hypervisor exit programs, 100+ VM fleets, regulated / air-gapped rollouts |
| **Support** | GitHub Issues &amp; Discussions | SLA, [sales@zyvor.dev](mailto:sales@zyvor.dev), migration workshops, professional services |
| **What you get** | Full CLI/TUI tooling, self-hosted consoles, Helm charts — the same codebase Enterprise runs | Same codebase + priority fixes, guided playbooks, hardened reference architectures, fleet automation |

### Community Edition — source & GitHub Pages

| Product | What it does | Source | Docs |
|:---|:---|:---|:---|
| **Transiva** | Enterprise workload mobility starts with honest offline VM export | [repo](https://github.com/zyvorai/transiva) | [pages](https://zyvorai.github.io/transiva/) |
| **Scout** | Migration discovery and readiness before migration risk | [repo](https://github.com/zyvorai/scout) | [pages](https://zyvorai.github.io/scout/) |
| **Chimera** | Programmable infrastructure simulator for migration and automation tests (vSphere today) | [repo](https://github.com/zyvorai/chimera) | [pages](https://zyvorai.github.io/chimera/) |
| **GuestKit** | Offline VM intelligence and migration assurance: inspect disks, zero boot, zero agents | [repo](https://github.com/zyvorai/guestkit) | [pages](https://zyvorai.github.io/guestkit/) |
| **h2kvm** | Any hypervisor → KVM: convert offline, fix the guest, deploy with confidence | [repo](https://github.com/zyvorai/h2kvm) | — |
| **Edge Stack** | One map of the Zyvor edge line: landing page and suite CI | [repo](https://github.com/zyvorai/edge-stack) | [pages](https://zyvorai.github.io/edge-stack/) |
| **Kairon** | Real VMs, real Kubernetes, no virt-launcher: Kairon orchestrates, FluxVM executes | [repo](https://github.com/zyvorai/kairon) | [pages](https://zyvorai.github.io/kairon/) |
| **Zorvia** | Kubernetes VMs, run like a platform: CLI, TUI and web console on one API | [repo](https://github.com/zyvorai/zorvia) | [pages](https://zyvorai.github.io/zorvia/) |
| **FluxVM** | Run real VMs with a real API: one Rust control plane for Firecracker, Cloud Hypervisor, QEMU/KVM and the FluxVM hypervisor | [repo](https://github.com/zyvorai/fluxvm) | [pages](https://zyvorai.github.io/fluxvm/) |
| **Fabric** | Private cloud control plane for Linux: VMs, networking, storage and security over one daemon | [repo](https://github.com/zyvorai/fabric) | [pages](https://zyvorai.github.io/fabric/) |
| **Kryton** | One stable machine API, real Windows behind the provider boundary | [repo](https://github.com/zyvorai/kryton) | [pages](https://zyvorai.github.io/kryton/) |
| **Haven** | Identity for the private cloud: Keycloak + PostgreSQL as one product | [repo](https://github.com/zyvorai/haven) | [pages](https://zyvorai.github.io/haven/) |
| **Fleet** | Every site, still running: offline-first edge site control plane | [repo](https://github.com/zyvorai/fleet) | [pages](https://zyvorai.github.io/fleet/) |
| **Nodra** | Open edge runtime that keeps sites running when the cloud doesn't | [repo](https://github.com/zyvorai/nodra) | [pages](https://zyvorai.github.io/nodra/) |
| **Device Agent** | Linux hardware edge agent: discover the box, publish to Nodra, Fleet inventory | [repo](https://github.com/zyvorai/device-agent) | [pages](https://zyvorai.github.io/device-agent/) |
| **OTA** | Signed, recoverable device OS updates (RAUC A/B, Ed25519-signed releases) | [repo](https://github.com/zyvorai/ota) | [pages](https://zyvorai.github.io/ota/) |
| **Yard** | Open asset and operations platform | [repo](https://github.com/zyvorai/yard) | [pages](https://zyvorai.github.io/yard/) |
| **Netra** | See every packet's story, contain the bad ones: standalone eBPF observability and emergency control | [repo](https://github.com/zyvorai/netra) | [pages](https://zyvorai.github.io/netra/) |
| **Paqtra** | Why can't A reach B? Traces every flow and shows Cilium's verdict | [repo](https://github.com/zyvorai/paqtra) | [pages](https://zyvorai.github.io/paqtra/) |
| **Rivora** | eBPF-native load balancing for every environment | [repo](https://github.com/zyvorai/rivora) | [pages](https://zyvorai.github.io/rivora/) |
| **Shukra** | eBPF-powered runtime intelligence and security for KVM | [repo](https://github.com/zyvorai/shukra) | — |
| **Duvora** | DPU fleet control plane: plans, isolation, telemetry, incidents and evidence | [repo](https://github.com/zyvorai/duvora) | — |
| **Gryvia** | GPU is the new CPU. Gryvia is its scheduler | [repo](https://github.com/zyvorai/gryvia) | [pages](https://zyvorai.github.io/gryvia/) |
| **Solvor** | Drop a file, get answers, nothing leaves the cell: a native Mac app | [repo](https://github.com/zyvorai/solvor) | — |
| **netevd** | Kernel events → your scripts: Rust network event daemon | [repo](https://github.com/zyvorai/netevd) | [pages](https://zyvorai.github.io/netevd/) |
| **netctl** | Network configuration CLI for Linux | [repo](https://github.com/zyvorai/netctl) | [pages](https://zyvorai.github.io/netctl/) |
| **cloud-netconfig** | Automatic network configuration from cloud metadata (Azure, AWS, GCP) | [repo](https://github.com/zyvorai/cloud-netconfig) | [pages](https://zyvorai.github.io/cloud-netconfig/) |
| **Kairo** | Know the blast radius before you deploy: SAFE / REVIEW / BLOCK verdicts | [repo](https://github.com/zyvorai/kairo) | [pages](https://zyvorai.github.io/kairo/) |
| **KubeFlight** | Know what may break before you deploy: local-first Kubernetes preflight | [repo](https://github.com/zyvorai/kubeflight) | [pages](https://zyvorai.github.io/kubeflight/) |
| **Zoreon** | Ops chat: Mattermost is the tape, Zoreon is the product | [repo](https://github.com/zyvorai/zoreon) | [pages](https://zyvorai.github.io/zoreon/) |
| **Aurora** | Turn your technical product into an AI-powered salesperson | [repo](https://github.com/zyvorai/aurora) | — |
| **Atlas** | The world of storage, under one command | [repo](https://github.com/zyvorai/atlas) | — |
| **HyperCluster** | Kubernetes cluster lifecycle for bare metal and private cloud | [repo](https://github.com/zyvorai/hypercluster) | — |
| **ZySign** | Sign MCA eForms from your Mac with a USB DSC token, no emBridge | [repo](https://github.com/zyvorai/zysign) | — |
| **relay-edge** | IoT simulators and site context for Relay (farm, firewater, remote edge, fleet) | [repo](https://github.com/zyvorai/relay-edge) | [pages](https://zyvorai.github.io/relay-edge/) |
| **relay-edge-bridge** | Protocol-neutral IoT/industrial edge bridge for Relay (Modbus, MQTT, HTTP) | [repo](https://github.com/zyvorai/relay-edge-bridge) | [pages](https://zyvorai.github.io/relay-edge-bridge/) |
| **relay-pubsub** | Google Cloud Pub/Sub compatibility gateway for Relay | [repo](https://github.com/zyvorai/relay-pubsub) | [pages](https://zyvorai.github.io/relay-pubsub/) |
| **Iris** | The application operating layer for Kubernetes | [repo](https://github.com/zyvorai/iris) | — |
| **Janus** | Discrete-event simulator for Kubernetes-native GPU scheduling | [repo](https://github.com/zyvorai/janus) | — |
| **Argus** | AI-first test platform: requirements → Playwright tests → regression reports | [repo](https://github.com/zyvorai/argus) | — |

[Zyntra](https://github.com/zyvorai/zyntra) is source-available under the Zyvor Production License, not Apache-2.0.

**Get started:** [Demo](https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org) → [Axiom](https://zyvor.dev/axiom?utm_source=github&utm_medium=zyvorai_org) → [Pricing](https://zyvor.dev/pricing?utm_source=github&utm_medium=zyvorai_org) → [Talk to us](https://zyvor.dev/contact?utm_source=github&utm_medium=zyvorai_org)

**Learn more:** [zyvor.dev/docs](https://zyvor.dev/docs?utm_source=github&utm_medium=zyvorai_org) · [zyvor.dev/blog](https://zyvor.dev/blog?utm_source=github&utm_medium=zyvorai_org) · [Narrative repo](https://github.com/zyvorai/zyvorai)

Maintainers: [GitHub org settings](../GITHUB_ORG_SETTINGS.md) · [Lead tracking](../LEADS.md)

---

<p align="center">
  <b>Ready for production?</b><br/><br/>
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/▶_Watch_demo-cc420a?style=for-the-badge" alt="Demo"/></a>
  <a href="https://zyvor.dev/contact?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Talk_to_sales-16a34a?style=for-the-badge" alt="Sales"/></a>
</p>
