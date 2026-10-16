<table>
  <tr>
    <td width="125" align="center" valign="middle">
      <img src="./assets/sa-mark.svg" alt="Shubham Antil" width="105" />
    </td>
    <td align="center" valign="middle">
      <h1 align="center">Shubham Antil</h1>
      <p align="center">
        <b>Security Researcher</b><br/>
        Vulnerability Research · Product Security · Application Security
      </p>
    </td>
  </tr>
</table>

<p align="center">
  <a href="mailto:shbhm.antil@gmail.com"><img src="https://img.shields.io/badge/Email-shbhm.antil%40gmail.com-0B2035?style=for-the-badge&logo=gmail&logoColor=65E6D4" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/shubhamantil/"><img src="https://img.shields.io/badge/LinkedIn-shubhamantil-0B2035?style=for-the-badge&logo=linkedin&logoColor=65E6D4" alt="LinkedIn" /></a>
  <a href="https://github.com/shbhmantil"><img src="https://img.shields.io/badge/GitHub-shbhmantil-0B2035?style=for-the-badge&logo=github&logoColor=65E6D4" alt="GitHub" /></a>
</p>

## I turn security findings into engineering outcomes

I work across the full vulnerability lifecycle: understanding attack surfaces, auditing source code, building deterministic proof-of-concepts, validating findings with runtime evidence, coordinating disclosure, and verifying the final patch.

My background spans nearly six years across security research, product and application security, and smart-contract auditing. I currently research open-source software and build tooling that makes vulnerability discovery, reproduction, triage, and remediation more reliable.

<p align="center">
  <img src="https://img.shields.io/badge/3-Assigned%20CVEs-19C3C8?style=for-the-badge" alt="3 assigned CVEs" />
  <img src="https://img.shields.io/badge/19-Confirmed%20Findings-19C3C8?style=for-the-badge" alt="19 confirmed findings" />
  <img src="https://img.shields.io/badge/8-High%20Severity-19C3C8?style=for-the-badge" alt="8 high severity findings" />
  <img src="https://img.shields.io/badge/50%2B-Applications%20Secured-19C3C8?style=for-the-badge" alt="More than 50 applications secured" />
</p>

## Research focus

<table>
  <tr>
    <td width="50%" align="center" valign="top">
      <h3 align="center">🧠 Vulnerability research</h3>
      <p align="center">Memory corruption, use-after-free, out-of-bounds access, uninitialized memory, parsers, device models, kernel networking, and exploitability analysis.</p>
    </td>
    <td width="50%" align="center" valign="top">
      <h3 align="center">🛡️ Product security</h3>
      <p align="center">Threat modeling, secure design reviews, source-code analysis, vulnerability triage, severity assessment, patch review, and remediation validation.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center" valign="top">
      <h3 align="center">⚙️ Research engineering</h3>
      <p align="center">PoC and harness development, sanitizer-backed validation, crash minimization, regression testing, build orchestration, and AI-assisted research workflows.</p>
    </td>
    <td width="50%" align="center" valign="top">
      <h3 align="center">🔐 Application security</h3>
      <p align="center">Web, mobile, API and cloud assessments; secure SDLC; SAST/DAST; penetration testing; and developer-focused security automation.</p>
    </td>
  </tr>
</table>

## Selected public research

### Assigned CVEs

| ID | Surface | Vulnerability class | Reference |
|---|---|---|---|
| **CVE-2026-60161** | Oracle VM VirtualBox VMDK parsing | Host-side heap corruption | [Oracle Security Alert](https://www.oracle.com/security-alerts/cpujul2026.html) |
| **CVE-2026-71125** | Oracle VM VirtualBox CUE parsing | Out-of-bounds write | [Oracle Security Alert](https://www.oracle.com/security-alerts/cspuaug2026.html) |
| **CVE-2026-66022** | QEMU virtio-net transmit path | DMA re-entrancy / memory safety | [Debian tracker](https://security-tracker.debian.org/tracker/CVE-2026-66022) |

### Upstream remediation

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>Linux kernel</h4>
      Two networking findings resulted in accepted patches:
      <ul>
        <li><a href="https://git.kernel.org/pub/scm/linux/kernel/git/netdev/net.git/commit/?id=65cf6863606b0507a7c3bd1711317e4f5d6b8b7e">RDS/IB receive-fragment validation</a></li>
        <li><a href="https://git.kernel.org/pub/scm/linux/kernel/git/klassert/ipsec.git/commit/?id=e35a12dffd5da67b6ca12bd23eebdd0570592205">XFRM replay-notify initialization</a></li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>radare2</h4>
      Three sanitizer-reproduced memory-safety issues were fixed upstream:
      <ul>
        <li><a href="https://github.com/radareorg/radare2/issues/26790">APFS parser heap OOB write</a></li>
        <li><a href="https://github.com/radareorg/radare2/issues/26791">GDB remote parser use-after-free</a></li>
        <li><a href="https://github.com/radareorg/radare2/issues/26792">LZ4 handling heap OOB write</a></li>
      </ul>
    </td>
  </tr>
</table>

> **Disclosure boundary:** this profile includes only information that is already public and independently verifiable. Private reports, customer information, unpublished vendor details, embargoed references, and internal research systems are intentionally excluded.

## Research workflow

```text
Map the attack surface → Form a source-level hypothesis → Build a minimal trigger
        ↓                                                        ↓
Verify the patch ← Coordinate disclosure ← Prove root cause and impact
```

The goal is not merely to produce a crash. A useful report gives maintainers a reproducible trigger, strong evidence, a defensible impact assessment, and enough context to implement and validate the right fix.

## Tools and ecosystems

<p align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,python,rust,linux,bash,git,docker&theme=dark" alt="C, C++, Python, Rust, Linux, Bash, Git and Docker" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AddressSanitizer-0B2035?style=flat-square&logoColor=65E6D4" alt="AddressSanitizer" />
  <img src="https://img.shields.io/badge/KASAN%20%2F%20KMSAN-0B2035?style=flat-square&logo=linux&logoColor=65E6D4" alt="KASAN and KMSAN" />
  <img src="https://img.shields.io/badge/Fuzzing-0B2035?style=flat-square&logoColor=65E6D4" alt="Fuzzing" />
  <img src="https://img.shields.io/badge/Ghidra-0B2035?style=flat-square&logoColor=65E6D4" alt="Ghidra" />
  <img src="https://img.shields.io/badge/QEMU-0B2035?style=flat-square&logo=qemu&logoColor=65E6D4" alt="QEMU" />
  <img src="https://img.shields.io/badge/Solidity-0B2035?style=flat-square&logo=solidity&logoColor=65E6D4" alt="Solidity" />
  <img src="https://img.shields.io/badge/Threat%20Modeling-0B2035?style=flat-square&logoColor=65E6D4" alt="Threat modeling" />
  <img src="https://img.shields.io/badge/Secure%20Code%20Review-0B2035?style=flat-square&logoColor=65E6D4" alt="Secure code review" />
</p>

## Professional journey

`Security Researcher` **Octane Security** · May 2025–Present  
`Smart Contract Auditor` **QuillAudits** · Oct 2024–May 2025  
`Application Security Manager` **Star Health and Allied Insurance** · Jun 2022–Oct 2024  
`Associate Security Engineer` **Castellum Labs** · Dec 2020–Jun 2022

## GitHub activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=shbhmantil&show_icons=true&hide_border=true&bg_color=071522&title_color=65E6D4&text_color=C9D7E3&icon_color=19C3C8" alt="Shubham's GitHub statistics" height="155" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=shbhmantil&layout=compact&hide_border=true&bg_color=071522&title_color=65E6D4&text_color=C9D7E3" alt="Most-used languages" height="155" />
</p>

<p align="center">
  Interested in product security, application security, or vulnerability research?<br/>
  <a href="mailto:shbhm.antil@gmail.com"><b>Let’s talk</b></a>
</p>
