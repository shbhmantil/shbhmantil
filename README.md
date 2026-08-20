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

Security researcher focused on **hypervisor and low-level memory-safety
vulnerabilities**. I hunt for bugs in virtualization and emulation stacks
(VirtualBox, QEMU) and system software, and disclose them through coordinated
vendor disclosure. My work has led to **3 assigned CVEs** across Oracle and
QEMU.

- 🏢 Currently: Security Researcher at **Octane Security**
- 🎯 Focus: hypervisor security, memory corruption (heap/OOB), virtual device emulation, fuzzing
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
