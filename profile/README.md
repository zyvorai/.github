<!-- utm: github / hypersdk_org (in href only) -->

<p align="center">
  <a href="https://zyvor.dev?utm_source=github&utm_medium=hypersdk_org">
    <img src="https://zyvor.dev/img/zavor-logo.webp" alt="Zyvor AI Labs — HyperSDK Platform" width="260">
  </a>
</p>

<h3 align="center">HyperSDK Platform · Zeus suite</h3>
<p align="center"><sub>Post-VMware infrastructure · Enterprise VM migration · by Zyvor AI Labs</sub></p>

<p align="center">
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/▶_Watch_demo-F97316?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch demo"/></a>
  <a href="https://dashboard.zyvor.dev?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/Live_dashboard-8B5CF6?style=for-the-badge&logo=grafana&logoColor=white" alt="Dashboard"/></a>
  <a href="https://zyvor.dev/contact?intent=demo&utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/Book_engineering_call-22C55E?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book call"/></a>
  <a href="https://github.com/sponsors/ssahani?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/Sponsor_ssahani-ea4aaa?style=for-the-badge&logo=github-sponsors&logoColor=white" alt="Sponsor"/></a>
  <a href="mailto:sales@zyvor.dev"><img src="https://img.shields.io/badge/sales@zyvor.dev-2563EB?style=for-the-badge&logo=gmail&logoColor=white" alt="Sales"/></a>
</p>

<p align="center">
  <code>VMware → KVM → KubeVirt</code> · <b>96.8%</b> first-boot · <b>12</b> products · <b>2,000+</b> APIs · <b>400+</b> dashboard views
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/hypersdk/hypersdk?style=flat-square&logo=github&label=Stars&labelColor=18181B&color=F97316" alt="Stars"/>
  <img src="https://img.shields.io/github/forks/hypersdk/hypersdk?style=flat-square&logo=github&label=Forks&labelColor=18181B&color=F97316" alt="Forks"/>
  <img src="https://img.shields.io/badge/CE_repos-3-18181B?style=flat-square&labelColor=F97316" alt="CE repos"/>
  <img src="https://img.shields.io/badge/Providers-10-06B6D4?style=flat-square&labelColor=18181B" alt="Providers"/>
  <img src="https://img.shields.io/badge/First_boot-96.8%25-22C55E?style=flat-square&labelColor=18181B" alt="First boot"/>
</p>

---

## Migrate a VM in 60 seconds

```bash
# Production-style cutover — Community Edition preview
$ hyperctl export --provider vmware --vm prod-db-01 --target kvm
→ Discovered (4 vCPU · 32 GiB · 420 GB)     ✓
→ Streamed export with integrity checks       ✓
→ hyper2kvm: QCOW2 + VirtIO + bootloader      ✓
→ GuestKit: guest validated offline           ✓
→ First boot on KVM                           ✓  6.8s

# Fleet migrations, SLAs, air-gap, VMware exit programs → talk to Zyvor
```

<p align="center">
  <img src="https://raw.githubusercontent.com/hypersdk/.github/main/profile/assets/hypersdk-dashboard.jpg" alt="HyperSDK live dashboard" width="92%"/>
</p>

<p align="center">
  <b>See the real platform first</b> — migration video, live dashboard, optional 30‑min engineering session<br/>
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=hypersdk_org"><b>Demo</b></a>
  ·
  <a href="https://dashboard.zyvor.dev?utm_source=github&utm_medium=hypersdk_org"><b>Dashboard</b></a>
  ·
  <a href="https://zyvor.dev/contact?utm_source=github&utm_medium=hypersdk_org"><b>Contact</b></a>
</p>

---

## What makes this different

<table>
<tr>
<td width="33%" align="center" valign="top">

### 🎯 One pipeline
Not 6 vendors. **Export → convert → fix → deploy → operate** in a single Zeus suite.

</td>
<td width="33%" align="center" valign="top">

### ⚡ 96.8% first boot
Automated **VirtIO**, bootloader repair, Windows & Linux — migrations that actually finish.

</td>
<td width="33%" align="center" valign="top">

### 🔒 Enterprise-ready
**SOC2-ready** · RBAC/SSO · audit logs · **air-gapped** · regulated industries.

</td>
</tr>
</table>

---

## Zeus suite · 12 products

```
   ┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
   │  HyperSDK   │───▶│  hyper2kvm  │───▶│  GuestKit   │───▶│   Aether    │
   │   Export    │    │   Convert   │    │   Inspect   │    │   Deploy    │
   └─────────────┘    └─────────────┘    └─────────────┘    └──────┬──────┘
                                                                     │
                    ┌─────────────┐    ┌─────────────┐    ┌─────────▼──────┐
                    │ PacketWolf  │◀───│     v9s     │◀───│  VMRogue · …   │
                    │   Observe   │    │   Manage    │    │  Machina · Forge│
                    └─────────────┘    └─────────────┘    └────────────────┘
```

<p align="center">
  <a href="https://zyvor.dev/hypersdk?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/HyperSDK-export-18181B?style=flat-square&logo=kubernetes&logoColor=F97316"/></a>
  <a href="https://zyvor.dev/hyper2kvm?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/hyper2kvm-convert-18181B?style=flat-square&logo=python&logoColor=F97316"/></a>
  <a href="https://zyvor.dev/guestkit?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/GuestKit-inspect-18181B?style=flat-square&logo=rust&logoColor=F97316"/></a>
  <a href="https://zyvor.dev/v9s?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/v9s-KubeVirt-18181B?style=flat-square&logo=kubernetes&logoColor=8B5CF6"/></a>
  <a href="https://zyvor.dev/packetwolf?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/PacketWolf-eBPF-18181B?style=flat-square&logo=linux&logoColor=8B5CF6"/></a>
  <a href="https://zyvor.dev/docs/products?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/+_7_more-products-F97316?style=flat-square"/></a>
</p>

---

## Built for every source · every target

<p align="center">
  <img src="https://img.shields.io/badge/VMware-vSphere-607078?style=for-the-badge&logo=vmware&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hyper--V-0078D4?style=for-the-badge&logo=windows&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenStack-ED1944?style=for-the-badge&logo=openstack&logoColor=white"/>
  <img src="https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white"/>
  <img src="https://img.shields.io/badge/KubeVirt-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
</p>

---

## Outcomes teams report

| Metric | Result |
|:-------|:-------|
| Fleet migration | **350 VMs** in **6 weeks** |
| Cost | **$1.2M** / yr saved · **$720K** cloud spend cut |
| Economics | **$100/VM/yr** vs **$1,200–5,000** VMware typical |
| Reliability | **96.8%** first-boot · near-zero cutover downtime |

> *"Every VM booted on the first try — zero downtime across 500 VMs."*  
> — Director of IT Operations, federal agency  
> [More case studies →](https://zyvor.dev/case-studies?utm_source=github&utm_medium=hypersdk_org)

<p align="center">
  <a href="https://zyvor.dev/vmware-exit?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/VMware_exit_program-F97316?style=for-the-badge"/></a>
  <a href="https://zyvor.dev/roi?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/ROI_calculator-22C55E?style=for-the-badge"/></a>
  <a href="https://zyvor.dev/pricing?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/Enterprise_pricing-2563EB?style=for-the-badge"/></a>
</p>

---

## ⚠️ You're on GitHub — that's Community Edition

| ✅ Fine for CE | 🏢 Contact Zyvor for |
|:---|:---|
| Labs, CI, single-VM experiments | VMware exit · **100+ VMs** · SLAs |
| Trying export / convert / guest tools | Air-gapped · compliance packs |
| Open-source contributors | Architecture review · cutover planning |

**CE repos:** [hypersdk](https://github.com/hypersdk/hypersdk) · [hyper2kvm](https://github.com/hypersdk/hyper2kvm) · [guestkit](https://github.com/hypersdk/guestkit)  

**Start here (sales funnel):** [Demo](https://zyvor.dev/demo?utm_source=github&utm_medium=hypersdk_org) → [ROI](https://zyvor.dev/roi?utm_source=github&utm_medium=hypersdk_org) → [Pricing](https://zyvor.dev/pricing?utm_source=github&utm_medium=hypersdk_org) → [Contact](https://zyvor.dev/contact?utm_source=github&utm_medium=hypersdk_org)

Maintainers: [GitHub org settings](../GITHUB_ORG_SETTINGS.md) · [Lead tracking](../LEADS.md)

---

<p align="center">
  <b>Ready for production?</b><br/><br/>
  <a href="https://zyvor.dev/demo?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/▶_Watch_demo-F97316?style=for-the-badge" alt="Demo"/></a>
  <a href="https://zyvor.dev/contact?utm_source=github&utm_medium=hypersdk_org"><img src="https://img.shields.io/badge/Talk_to_sales-22C55E?style=for-the-badge" alt="Sales"/></a>
</p>
