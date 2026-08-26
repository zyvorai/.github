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
  Migrate off proprietary hypervisors &amp; HCI platforms, run on Kubernetes &amp; KubeVirt, operate at the edge —
  one API contract across every layer.<br/>
  <sub><a href="https://zyvor.dev?utm_source=github&utm_medium=zyvorai_org">Zyvor</a> · zyvor.dev</sub>
</p>

<p align="center">
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/▶_Watch_demo-cc420a?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch demo"/></a>
  <a href="https://dashboard.zyvor.dev?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Live_dashboard-1f2937?style=for-the-badge&logo=grafana&logoColor=white" alt="Dashboard"/></a>
  <a href="https://zyvor.dev/contact?intent=demo&utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Book_engineering_call-16a34a?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book call"/></a>
  <a href="mailto:sales@zyvor.dev"><img src="https://img.shields.io/badge/sales%40zyvor.dev-2563eb?style=for-the-badge&logo=gmail&logoColor=white" alt="Sales"/></a>
</p>

<p align="center">
  <a href="https://github.com/zyvorai/transiva/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/transiva?style=flat-square&logo=github&label=Stars&labelColor=18181B&color=cc420a" alt="Stars"/></a>
  <a href="https://github.com/zyvorai/h2kvm/stargazers"><img src="https://img.shields.io/github/stars/zyvorai/h2kvm?style=flat-square&logo=github&label=h2kvm&labelColor=18181B&color=cc420a" alt="h2kvm"/></a>
  <img src="https://img.shields.io/badge/Apache--2.0-core_toolkit-18181B?style=flat-square&labelColor=18181B" alt="Apache-2.0"/>
  <img src="https://img.shields.io/badge/First_boot-96.8%25-16a34a?style=flat-square&labelColor=18181B" alt="First boot"/>
</p>

---

## Try it in 60 seconds

```bash
# Community Edition preview — export, convert, and validate a VM offline
$ transivactl export --provider enterprise-hypervisor --vm prod-db-01 --target kvm
→ Discovered (4 vCPU · 32 GiB · 420 GB)       ✓
→ Streamed export with integrity checks       ✓
→ k2kvm / h2kvm: QCOW2 + VirtIO + bootloader  ✓
→ GuestKit: guest validated offline           ✓
→ First boot on KVM                           ✓  6.8s

# Fleet migrations, SLAs, air-gapped rollouts → talk to Zyvor
```

<p align="center">
  <b>See the real platform first</b> — migration video, live dashboard, an optional 30-minute engineering session<br/>
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org"><b>Demo</b></a>
  ·
  <a href="https://dashboard.zyvor.dev?utm_source=github&utm_medium=zyvorai_org"><b>Dashboard</b></a>
  ·
  <a href="https://zyvor.dev/contact?utm_source=github&utm_medium=zyvorai_org"><b>Contact</b></a>
</p>

---

## What makes this different

<table>
<tr>
<td width="33%" align="center" valign="top">

### One pipeline
Not a stack of point tools. **Export → convert → fix → deploy → operate**, one suite, one API contract.

</td>
<td width="33%" align="center" valign="top">

### 96.8% first boot
Automated **VirtIO** injection and bootloader repair, Windows &amp; Linux — migrations that actually finish.

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
| **Migrate** | Discover, export, convert, and assure workloads off proprietary hypervisors, HCI platforms, and public cloud | [Transiva](https://zyvor.dev/zyvor-ai-platform?utm_source=github&utm_medium=zyvorai_org) · [k2kvm](https://zyvor.dev/k2kvm?utm_source=github&utm_medium=zyvorai_org) · [GuestKit](https://zyvor.dev/guestkit?utm_source=github&utm_medium=zyvorai_org) |
| **Run** | Operate VMs and applications on Kubernetes, KubeVirt, and libvirt from one control plane | [Zeus OS](https://zyvor.dev/zeus-os?utm_source=github&utm_medium=zyvorai_org) · [Veyron](https://zyvor.dev/veyron?utm_source=github&utm_medium=zyvorai_org) · [Hermes](https://zyvor.dev/hermes?utm_source=github&utm_medium=zyvorai_org) · [Machina](https://zyvor.dev/machina?utm_source=github&utm_medium=zyvorai_org) |
| **Operate** | Deploy anywhere, see every packet, schedule GPUs, automate bare metal, prove reliability | [Aether](https://zyvor.dev/aether?utm_source=github&utm_medium=zyvorai_org) · [PacketWolf](https://zyvor.dev/packetwolf?utm_source=github&utm_medium=zyvorai_org) · [Forge](https://zyvor.dev/forge?utm_source=github&utm_medium=zyvorai_org) |
| **Scale** | Stand up clusters and sign regulated documents — the bookends of the platform | [HyperCluster](https://zyvor.dev/hypercluster?utm_source=github&utm_medium=zyvorai_org) · [ZySign](https://zyvor.dev/zysign?utm_source=github&utm_medium=zyvorai_org) |
| **Community Edition** | Apache-2.0 host networking, GPU scheduling simulation, and AI-driven QA — maintained in the open, right here | ↓ see below |

<p align="center"><a href="https://zyvor.dev/products?utm_source=github&utm_medium=zyvorai_org">Full product catalogue →</a> · <a href="https://zyvor.dev/compare?utm_source=github&utm_medium=zyvorai_org">Compare all products →</a></p>

---

## Built for every source, every target

<p align="center">
  <img src="https://img.shields.io/badge/Enterprise_hypervisors-18181B?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/HCI_platforms-18181B?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Windows_hypervisors-18181B?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Oracle_Cloud-F80000?style=for-the-badge&logo=oracle&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenStack-ED1944?style=for-the-badge&logo=openstack&logoColor=white"/>
  <img src="https://img.shields.io/badge/Alibaba_Cloud-FF6A00?style=for-the-badge&logo=alibabacloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/KubeVirt-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
</p>

Integration targets today — see the [full migration paths](https://zyvor.dev/products?utm_source=github&utm_medium=zyvorai_org) and [real customer case studies](https://zyvor.dev/case-studies?utm_source=github&utm_medium=zyvorai_org).

<p align="center">
  <a href="https://zyvor.dev/hypervisor-exit?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Hypervisor_exit_program-cc420a?style=for-the-badge"/></a>
  <a href="https://zyvor.dev/roi?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/ROI_calculator-16a34a?style=for-the-badge"/></a>
  <a href="https://zyvor.dev/pricing?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Enterprise_pricing-2563eb?style=for-the-badge"/></a>
</p>

---

## Open source vs Enterprise

Everything below is real, working, Apache-2.0 source — not a crippled trial. Enterprise is support, scale programs, and hardened deployments on top of it, not features withheld from the repo.

| | Open source (these repos) | Enterprise ([zyvor.dev](https://zyvor.dev?utm_source=github&utm_medium=zyvorai_org)) |
|:---|:---|:---|
| **Good for** | Labs, CI gates, single-VM / small-fleet migrations, contributing | Hypervisor exit programs, 100+ VM fleets, regulated / air-gapped rollouts |
| **Support** | GitHub Issues &amp; Discussions | SLA, [sales@zyvor.dev](mailto:sales@zyvor.dev), migration workshops, professional services |
| **What you get** | Full CLI/TUI tooling, self-hosted consoles, Helm charts — the same codebase Enterprise runs | Same codebase + priority fixes, guided playbooks, hardened reference architectures, fleet automation |

**Open source repos:**
[transiva](https://github.com/zyvorai/transiva) ·
[h2kvm](https://github.com/zyvorai/h2kvm) ·
[guestkit](https://github.com/zyvorai/guestkit) ·
[ephemera](https://github.com/zyvorai/ephemera) ·
[janus](https://github.com/zyvorai/janus) ·
[argus](https://github.com/zyvorai/argus) ·
[cloud-netconfig](https://github.com/zyvorai/cloud-netconfig) ·
[netctl](https://github.com/zyvorai/netctl) ·
[netevd](https://github.com/zyvorai/netevd) ·
[relay](https://github.com/zyvorai/relay)

**Get started:** [Demo](https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org) → [ROI calculator](https://zyvor.dev/roi?utm_source=github&utm_medium=zyvorai_org) → [Pricing](https://zyvor.dev/pricing?utm_source=github&utm_medium=zyvorai_org) → [Talk to us](https://zyvor.dev/contact?utm_source=github&utm_medium=zyvorai_org)

**Learn more:** [zyvor.dev/docs](https://zyvor.dev/docs?utm_source=github&utm_medium=zyvorai_org) · [zyvor.dev/blog](https://zyvor.dev/blog?utm_source=github&utm_medium=zyvorai_org) · [zyvor.dev/case-studies](https://zyvor.dev/case-studies?utm_source=github&utm_medium=zyvorai_org)

Maintainers: [GitHub org settings](../GITHUB_ORG_SETTINGS.md) · [Lead tracking](../LEADS.md)

---

<p align="center">
  <b>Ready for production?</b><br/><br/>
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/▶_Watch_demo-cc420a?style=for-the-badge" alt="Demo"/></a>
  <a href="https://zyvor.dev/contact?utm_source=github&utm_medium=zyvorai_org"><img src="https://img.shields.io/badge/Talk_to_sales-16a34a?style=for-the-badge" alt="Sales"/></a>
</p>
