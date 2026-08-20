<h1 align="center">Hi, I'm Shubham Antil 👋</h1>

<p align="center">
  <b>Security Researcher</b> · Vulnerability Research · Hypervisor &amp; Memory-Safety
</p>

<p align="center">
  <a href="mailto:shubham@octane.security"><img src="https://img.shields.io/badge/Email-shubham%40octane.security-informational?style=flat-square&logo=gmail&logoColor=white"></a>
  <a href="https://github.com/shbhmantil"><img src="https://img.shields.io/badge/GitHub-shbhmantil-181717?style=flat-square&logo=github&logoColor=white"></a>
</p>

---

## 🔎 About

Security Engineer with 5+ years of experience spanning **smart-contract
auditing**, **application security**, and **low-level vulnerability research**.
I audit DeFi protocols, hunt for bugs in virtualization and emulation stacks
(VirtualBox, QEMU) and system software, and disclose them through coordinated
vendor disclosure. My work has led to **3 assigned CVEs** across Oracle and
QEMU.

- 🏢 Currently: Security Researcher at **Octane Security**
- 🎯 Focus: hypervisor & memory corruption (heap/OOB), smart-contract security, code review, SAST/DAST
- 📫 Reach me: [shubham@octane.security](mailto:shubham@octane.security)

---

## 🧾 Assigned CVEs

> Published, credited vulnerabilities I discovered and disclosed.

| CVE | Finding | Vendor | Type | Status |
|-----|---------|--------|------|--------|
| **[CVE-2026-60161](https://nvd.nist.gov/vuln/detail/CVE-2026-60161)** | VirtualBox VMDK `streamOptimized` heap buffer overflow | Oracle | Heap Buffer Overflow | ✅ Confirmed |
| **[CVE-2026-71125](https://nvd.nist.gov/vuln/detail/CVE-2026-71125)** | VirtualBox CUE `TRACK 00` out-of-bounds write | Oracle | Out-of-Bounds Write | ✅ Confirmed |
| **[CVE-2026-66022](https://nvd.nist.gov/vuln/detail/CVE-2026-66022)** | QEMU virtio-net `tx_bh` DMA reentrancy | QEMU | DMA Reentrancy / Use-After-Free | ✅ Confirmed |

<details>
<summary><b>CVE-2026-60161 — VirtualBox VMDK streamOptimized heap buffer overflow</b></summary>

A heap buffer overflow in Oracle VirtualBox's VMDK `streamOptimized` disk-image
parser. Crafted grain-table/metadata in a malicious VMDK image causes an
oversized write past a heap allocation while decompressing/parsing image data,
corrupting adjacent heap memory — a path toward guest-to-host memory corruption.

</details>

<details>
<summary><b>CVE-2026-71125 — VirtualBox CUE TRACK 00 out-of-bounds write</b></summary>

An out-of-bounds write in VirtualBox's CUE sheet parser. A malformed `TRACK 00`
entry drives an index/offset outside the intended bounds, producing an
attacker-influenced out-of-bounds write when the image is mounted/parsed.

</details>

<details>
<summary><b>CVE-2026-66022 — QEMU virtio-net tx_bh DMA reentrancy</b></summary>

A DMA-reentrancy flaw in QEMU's virtio-net device. Reentrant access through the
`tx_bh` transmit bottom-half path re-enters device processing during DMA,
leading to inconsistent device state and a use-after-free condition reachable
from a malicious guest.

</details>

---

## 💼 Experience

**Security Researcher** — Octane Security · *2025 May – Present*

- Low-level vulnerability research on virtualization and emulation stacks (VirtualBox, QEMU), resulting in **3 assigned CVEs**.
- Memory-safety analysis of virtual disk-image parsers and device models — heap buffer overflows, out-of-bounds writes, and DMA-reentrancy / use-after-free conditions.

**Smart Contract Auditor** — QuillAudits · *2024 Oct – 2025 May*

- Conducted comprehensive solo audits for **Magpie Cross-Chain Bridge, Zoth Pool, Nordek, NFTFN, De.Fi** and others, assessing DeFi protocols involving AMMs, staking pools, vesting, bridges, and ERC-20/ERC-721.
- Performed risk assessments across ERC-20 tokens, NFT marketplaces, and DeFi lending/borrowing platforms.
- Identified and remediated critical flaws — reentrancy, improper accounting, precision errors, and inadequate reward calculations — strengthening client security frameworks.
- Audited projects built in **Cairo (Starknet)** and **FunC (TON)**.

**Application Security Manager** — Star Health and Allied Insurance · *2022 Jun – 2024 Oct*

- Built and rolled out an automated security testing framework covering 50+ applications (Bash & Python).
- Led periodic penetration testing, red-team exercises, and pre-release security assessments (PRSA); triaged, ranked, and prioritized vulnerabilities and drove timely remediation.
- Revised application security standards and procedures for **IRDAI** compliance.
- Owned risk management and threat modeling across organizational assets.

**Associate Security Engineer** — Castellum Labs · *2020 Dec – 2022 Jun*

- Delivered VAPT for web applications, mobile apps, and APIs, communicating findings in professional client reports.
- Researched and curated a collection of open-source security tooling.
- Designed a fully orchestrated, automated platform for web/mobile application security testing (Python), reducing testing time and effort.

---

## 🎓 Education & Certifications

- **M.Sc. Cyber Forensics & Information Security** — University of Madras *(2022–2024)*
- **B.Sc. Computer Science** — Maharishi Dayanand University *(2017–2020)*
- **Certified Ethical Hacker (Practical)** — EC-Council · **IBM Cybersecurity Analyst** — Coursera · **HTB Pro Lab: Dante**

---

## 🛠️ Skills & Tooling

<p align="left">
  <img src="https://img.shields.io/badge/-C-A8B9CC?style=flat-square&logo=c&logoColor=black">
  <img src="https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=cplusplus&logoColor=white">
  <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white">
  <img src="https://img.shields.io/badge/-QEMU-FF6600?style=flat-square&logo=qemu&logoColor=white">
  <img src="https://img.shields.io/badge/-VirtualBox-183A61?style=flat-square&logo=virtualbox&logoColor=white">
  <img src="https://img.shields.io/badge/-Ghidra-CE1126?style=flat-square">
  <img src="https://img.shields.io/badge/-Fuzzing-4B0082?style=flat-square">
  <img src="https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black">
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=shbhmantil&show_icons=true&theme=transparent&hide_border=true" alt="GitHub stats" height="150">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=shbhmantil&layout=compact&theme=transparent&hide_border=true" alt="Top languages" height="150">
</p>

---

<p align="center"><i>Interested in my research? Reach out at <a href="mailto:shubham@octane.security">shubham@octane.security</a>.</i></p>
