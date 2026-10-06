<!-- ============================================================
     OMKAR SAHNI — GITHUB PROFILE
     Security Researcher • Firmware RE • Android • Web • IoT
============================================================= -->

<div align="center">

<img src="./banner.png" alt="Omkar Sahni — Security Researcher" width="100%" />

<br/>

<a href="https://leakhunterx.com">
  <img src="https://img.shields.io/badge/LeakHunterX-E11D48?style=for-the-badge&labelColor=0D1117" />
</a>
<a href="https://hackerone.com/omkar_sahni">
  <img src="https://img.shields.io/badge/HackerOne-181717?style=for-the-badge&logo=hackerone&logoColor=white" />
</a>
<a href="https://www.linkedin.com/in/omkar-sahni-89b952324">
  <img src="https://img.shields.io/badge/LinkedIn-181717?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="https://github.com/Omkar443">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

<img
  src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2400&pause=800&color=F43F5E&center=true&vCenter=true&width=900&lines=Firmware+Reverse+Engineering;Android+Security+Research;Vulnerability+Research;IoT+%26+Embedded+Security;Building+LeakHunterX;Break+assumptions.+Build+better+systems."
  alt="Research Focus"
/>

</div>

---

## `$ whoami`

<table>
<tr>

<td width="58%" valign="top">

Independent security researcher focused on **firmware reverse engineering, Android security, vulnerability research, IoT / embedded security, and offensive security engineering**.

I work across the full vulnerability-research lifecycle:

**reconnaissance → reverse engineering → dynamic analysis → impact validation → responsible disclosure → remediation verification**

Currently building **[LeakHunterX](https://leakhunterx.com)**, a distributed secret-scanning platform designed to perform security analysis while keeping customer source code local.

</td>

<td width="42%" valign="top">

```bash
omkar@research:~$ whoami

[+] Security Researcher
[+] Vulnerability Researcher
[+] Firmware Reverse Engineer
[+] Security Tool Builder
[+] Founder @ LeakHunterX
```

</td>

</tr>
</table>

<div align="center">

`FIRMWARE RE` • `ANDROID SECURITY` • `WEB / API` • `IoT` • `SECURITY AUTOMATION`

</div>

<br/>

---

# 🛡️ Selected Security Research

<div align="center">

<img src="./research.png" alt="Selected Security Research" width="100%" />

</div>

<br/>

<table>
<tr>

<td width="33%" valign="top">

### 📡 TP-Link Archer C7 v5

**2 CVE submissions pending with MITRE**

`CWE-78` • `CWE-321`

Full firmware-analysis chain:

`Binwalk → Lua/LuCI RE → QEMU ARM → Dynamic Analysis`

Research included:

- Command-injection path with unauthenticated RCE impact
- Hardcoded RSA private-key recovery
- Root-level execution validation
- Responsible disclosure
- End-of-Life confirmation from vendor

</td>

<td width="33%" valign="top">

### 🏆 TikTok

**$4,500 Responsible Disclosure Bounty**

Research lifecycle:

`Discovery → Validation → PoC → Report → Triage → Remediation`

Developed a sanitized proof of concept demonstrating impact and completed the coordinated disclosure process through remediation verification.

</td>

<td width="33%" valign="top">

### 📱 Coinbase Wallet

**Android Security Research**

Research areas included:

- BIP-39 seed phrase exposure
- `AccessibilityService`
- Controlled PoC APK
- Exfiltration validation
- Multi-device testing
- Mitigation analysis

Evaluated behavior around:

`importantForAccessibility="no-hide-descendants"`

</td>

</tr>
</table>

---

## 🔬 Research Methodology

```text
┌──────────────┐
│ TARGET / FW  │
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ EXTRACTION   │  Binwalk / Filesystem
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ STATIC RE    │  Lua / LuCI / ASM
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ EMULATION    │  QEMU / ARM / MIPS
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ DYNAMIC      │  Runtime behavior
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ VALIDATION   │  Exploit / Impact
└──────┬───────┘
       │
       ▼
┌──────────────┐
│ DISCLOSURE   │  Vendor / Program
└──────────────┘
```

<div align="center">

`EXPLORE // REVERSE // ANALYZE // EXPLOIT // DISCLOSE`

</div>

---

# ⚡ Currently Building — LeakHunterX

<div align="center">

<img src="./leakhunterx.png" alt="LeakHunterX Architecture" width="100%" />

<br/>

<a href="https://leakhunterx.com">
  <img src="https://img.shields.io/badge/VISIT_LEAKHUNTERX-E11D48?style=for-the-badge&labelColor=0D1117" />
</a>

</div>

<br/>

### Distributed Secret-Scanning Infrastructure

**LeakHunterX** is a distributed security platform designed to detect exposed credentials while keeping source code on the user's machine.

<table>
<tr>

<td align="center"><b>🔐 Local First</b><br/><sub>Source remains on-device</sub></td>
<td align="center"><b>🔎 50+ Patterns</b><br/><sub>Secret detection rules</sub></td>
<td align="center"><b>⚡ Real-Time</b><br/><sub>Distributed scanning</sub></td>
<td align="center"><b>📊 Reporting</b><br/><sub>JSON / CSV / PDF</sub></td>

</tr>
</table>

### Architecture

```text
                  ┌──────────────────────┐
                  │ LOCAL SCANNER AGENT  │
                  │ Source stays local   │
                  └──────────┬───────────┘
                             │
                  Authenticated WebSocket
                             │
                             ▼
                  ┌──────────────────────┐
                  │    FASTAPI BACKEND   │
                  └───────┬───────┬──────┘
                          │       │
                     ┌────▼───┐ ┌─▼──────────┐
                     │ REDIS  │ │ POSTGRESQL │
                     └────┬───┘ └─┬──────────┘
                          │       │
                          └───┬───┘
                              ▼
                  ┌──────────────────────┐
                  │ REAL-TIME DASHBOARD  │
                  │ Reports / Analytics  │
                  └──────────────────────┘
```

<div align="center">

![FastAPI](https://img.shields.io/badge/FastAPI-111827?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-111827?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-111827?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-111827?style=flat-square&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-111827?style=flat-square&logo=python&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSockets-111827?style=flat-square)

</div>

---

# 🚀 Featured Projects

<div align="center">

<img src="./projects.png" alt="Featured Security Projects" width="100%" />

<br/>

<a href="https://github.com/Omkar443/nyx">
  <img src="https://img.shields.io/badge/NYX-E11D48?style=for-the-badge&logo=github&logoColor=white&labelColor=0D1117" />
</a>
<a href="https://github.com/Omkar443/ProbeRaptor">
  <img src="https://img.shields.io/badge/ProbeRaptor-E11D48?style=for-the-badge&logo=github&logoColor=white&labelColor=0D1117" />
</a>
<a href="https://github.com/Omkar443/leakhunterx-agent">
  <img src="https://img.shields.io/badge/LHX_Agent-E11D48?style=for-the-badge&logo=github&logoColor=white&labelColor=0D1117" />
</a>
<a href="https://github.com/Omkar443/Kioptrix-Level1-Writeup">
  <img src="https://img.shields.io/badge/Kioptrix-E11D48?style=for-the-badge&logo=github&logoColor=white&labelColor=0D1117" />
</a>

</div>

<br/>

<table>
<tr>

<td width="25%" valign="top">

### 🧠 NYX

AI security-research platform combining:

- Attack-surface intelligence
- Dynamic analysis
- AI research agents
- Validation workflows
- Knowledge-driven automation

</td>

<td width="25%" valign="top">

### 🛰️ ProbeRaptor

Original reconnaissance framework featuring:

- Subdomain brute forcing
- CT-log analysis
- Parallel port scanning
- Target scoring
- JSON reporting

</td>

<td width="25%" valign="top">

### 🤖 LeakHunterX Agent

Autonomous research agent focused on:

- Reconnaissance
- Attack-surface analysis
- Vulnerability discovery
- Security automation

</td>

<td width="25%" valign="top">

### ⚔️ Kioptrix Level 1

Technical exploitation walkthrough covering:

- Reconnaissance
- Enumeration
- Exploitation
- Linux privilege escalation

</td>

</tr>
</table>

---

# ⚔️ Research Arsenal

<div align="center">

### `SECURITY RESEARCH`

![Firmware](https://img.shields.io/badge/Firmware_RE-111827?style=flat-square)
![Android](https://img.shields.io/badge/Android-111827?style=flat-square&logo=android&logoColor=white)
![Web Security](https://img.shields.io/badge/Web_Security-111827?style=flat-square)
![API Security](https://img.shields.io/badge/API_Security-111827?style=flat-square)
![IoT](https://img.shields.io/badge/IoT_/_Embedded-111827?style=flat-square)
![RF](https://img.shields.io/badge/802.11_/_RF-111827?style=flat-square)

### `SECURITY TOOLING`

![Burp](https://img.shields.io/badge/Burp_Suite-111827?style=flat-square)
![MobSF](https://img.shields.io/badge/MobSF-111827?style=flat-square)
![JADX](https://img.shields.io/badge/JADX-111827?style=flat-square)
![Binwalk](https://img.shields.io/badge/Binwalk-111827?style=flat-square)
![QEMU](https://img.shields.io/badge/QEMU-111827?style=flat-square&logo=qemu&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-111827?style=flat-square)
![Nmap](https://img.shields.io/badge/Nmap-111827?style=flat-square)
![Nessus](https://img.shields.io/badge/Nessus-111827?style=flat-square)
![Kali](https://img.shields.io/badge/Kali_Linux-111827?style=flat-square&logo=kalilinux&logoColor=white)

### `ENGINEERING`

![Python](https://img.shields.io/badge/Python-111827?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-111827?style=flat-square&logo=c&logoColor=white)
![Java](https://img.shields.io/badge/Java-111827?style=flat-square&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-111827?style=flat-square&logo=javascript&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-111827?style=flat-square&logo=postgresql&logoColor=white)
![MIPS](https://img.shields.io/badge/MIPS_Assembly-111827?style=flat-square)
![x86](https://img.shields.io/badge/x86_Assembly-111827?style=flat-square)

### `BACKEND / INFRA`

![FastAPI](https://img.shields.io/badge/FastAPI-111827?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-111827?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-111827?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-111827?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-111827?style=flat-square&logo=linux&logoColor=white)
![Git](https://img.shields.io/badge/Git-111827?style=flat-square&logo=git&logoColor=white)

</div>

---

# ⚡ Hardware → Security · Journey · Activity

<div align="center">

<img src="./journey.png" alt="Research Arsenal, Journey and GitHub Activity" width="100%" />

</div>

<br/>

<table>
<tr>

<td width="50%" valign="top">

### ⚡ Why the hardware background matters

My route into cybersecurity began with **Electrical & Electronics Engineering**.

That foundation now feeds directly into firmware and embedded research:

```text
Electrical Engineering
        ↓
Digital Logic
        ↓
Microprocessors
        ↓
Assembly
        ↓
Embedded Systems
        ↓
Firmware Reverse Engineering
        ↓
IoT Security
```

</td>

<td width="50%" valign="top">

### 🧭 Journey

```text
2018 ── Electrical & Electronics Engineering
  │
2023 ── Industrial Electrical Engineering
  │
2024 ── Computer Science / Cyber Security
  │
2025 ── Independent Security Research
  │
2025 ── Founder — LeakHunterX
  │
 NOW ── Building • Breaking • Researching
```

</td>

</tr>
</table>

---

# 📊 Live GitHub Activity

<div align="center">

<img
  width="49%"
  src="https://github-readme-stats.vercel.app/api?username=Omkar443&show_icons=true&hide_border=true&bg_color=0D1117&title_color=F43F5E&icon_color=F43F5E&text_color=C9D1D9&ring_color=F43F5E"
/>

<img
  width="49%"
  src="https://github-readme-stats.vercel.app/api/top-langs/?username=Omkar443&layout=compact&hide_border=true&bg_color=0D1117&title_color=F43F5E&text_color=C9D1D9"
/>

</div>

---

<details>
<summary><b>🎯 Current Research Focus</b></summary>

<br/>

```ini
[ RESEARCH ]

Firmware Security
Android Application Security
IoT / Embedded Security
Vulnerability Research
Reverse Engineering


[ BUILDING ]

LeakHunterX
Security Automation
Security Research Infrastructure
Open-Source Tooling


[ INTERESTED_IN ]

Firmware / Embedded Security
Android Security
Security Engineering
Vulnerability Research
IoT Security
Research Collaboration
```

</details>

<details>
<summary><b>🎓 Education & Engineering Background</b></summary>

<br/>

**B.Tech — Computer Science Engineering (Cyber Security)**  
Parul University

**Diploma — Electrical & Electronics Engineering**  
Korea Nepal Polytechnic Institute

**Former Sub Electrical Engineer — Varun Beverages**

Industrial systems, electrical maintenance, hardware fault diagnosis, microprocessor fundamentals, and circuit-level engineering now contribute to my embedded-security methodology.

</details>

---

# 📡 Connect

<div align="center">

### `LET'S BUILD A MORE SECURE DIGITAL WORLD`

<br/>

<a href="https://leakhunterx.com">
  <img src="https://img.shields.io/badge/LeakHunterX-E11D48?style=for-the-badge&labelColor=0D1117" />
</a>

<a href="https://hackerone.com/omkar_sahni">
  <img src="https://img.shields.io/badge/HackerOne-181717?style=for-the-badge&logo=hackerone&logoColor=white" />
</a>

<a href="https://www.linkedin.com/in/omkar-sahni-89b952324">
  <img src="https://img.shields.io/badge/LinkedIn-181717?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>

<a href="https://github.com/Omkar443">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

```text
omkar@research:~$ ./find-next-bug

[+] loading research environment...
[+] attack surface mapped...
[+] curiosity enabled...
[+] assumptions questioned...
[+] research never stops...

omkar@research:~$ █
```

<br/>

## `BREAK ASSUMPTIONS // BUILD BETTER SYSTEMS`

<sub>Firmware • Android • Web • IoT • Security Research</sub>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=rect&height=4&color=E11D48" width="100%" />

</div>
