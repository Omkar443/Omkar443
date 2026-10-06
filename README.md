<!--
=============================================================================
 OMKAR SAHNI — GITHUB PROFILE
 Security Researcher • Firmware RE • Android • Web • IoT
=============================================================================
-->

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&height=8&color=E11D48"/>

<br/>

<pre>
 // EXPLORE   // REVERSE   // ANALYZE   // EXPLOIT   // DISCLOSE
</pre>

# `OMKAR SAHNI`

### <code>SECURITY RESEARCHER</code>

#### `FIRMWARE RE`  |  `ANDROID SECURITY`  |  `WEB SECURITY`  |  `IoT`

<br/>

<table>
<tr>
<td align="center">
<b>🛡️ Vulnerability<br/>Research</b>
</td>
<td align="center">
<b>⚙️ Security<br/>Automation</b>
</td>
<td align="center">
<b>🎯 Bug Bounty<br/>Research</b>
</td>
<td align="center">
<b>🛠️ Security Tool<br/>Builder</b>
</td>
</tr>
</table>

<br/>

> ### `"Finding flaws in the systems that power our world."`

```bash
omkar@research:~$ ./hunt █
```

<p align="center">

<a href="https://leakhunterx.com">
<img src="https://img.shields.io/badge/🔥_LeakHunterX-E11D48?style=for-the-badge&labelColor=0D1117"/>
</a>

<a href="https://hackerone.com/omkar_sahni">
<img src="https://img.shields.io/badge/HackerOne-181717?style=for-the-badge&logo=hackerone&logoColor=white"/>
</a>

<a href="https://www.linkedin.com/in/omkar-sahni-89b952324">
<img src="https://img.shields.io/badge/LinkedIn-181717?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="https://github.com/Omkar443">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</p>

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&height=2&color=E11D48"/>

</div>

<br/>

# `$ whoami` <sub><code>█</code></sub>

<table>
<tr>

<td width="60%" valign="top">

Independent security researcher focused on **firmware reverse engineering, Android security, vulnerability research, IoT security, and offensive security engineering**.

My work spans the full vulnerability research lifecycle — from **static and dynamic analysis** through exploit development, responsible disclosure, and remediation verification.

Currently building **[LeakHunterX](https://leakhunterx.com)**, a distributed secret-scanning platform designed to analyze source code while keeping customer source files local.

</td>

<td width="40%" valign="top">

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

<br/>

<table>
<tr>
<td align="center"><b>🧬 Firmware RE</b><br/><sub>ARM / MIPS</sub></td>
<td align="center"><b>📱 Android Security</b><br/><sub>IPC / Intents</sub></td>
<td align="center"><b>🌐 Web & API</b><br/><sub>Offensive Research</sub></td>
<td align="center"><b>📡 IoT / Embedded</b><br/><sub>Hardware Security</sub></td>
<td align="center"><b>🧠 Automation</b><br/><sub>Python / Backend</sub></td>
<td align="center"><b>🎯 Bug Bounty</b><br/><sub>Vulnerability Research</sub></td>
</tr>
</table>

---

# 🛡️ Selected Security Research <sub><code>█</code></sub>

<table>
<tr>

<td width="33%" valign="top">

## 📡 TP-Link Archer C7 v5

### `2 CVE submissions pending with MITRE`

<p>
<img src="https://img.shields.io/badge/Firmware_RE-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/ARM-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/QEMU-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/Binwalk-111827?style=flat-square"/>
</p>

**CWE-78 — Command Injection**

Attacker-controlled input reaches a LuCI web-interface handler, resulting in **unauthenticated root-level command execution**.

**CWE-321 — Hardcoded RSA Key**

RSA private-key material was embedded within distributed firmware configuration.

### Research Chain

```text
Extraction
   ↓
Reverse Engineering
   ↓
QEMU Emulation
   ↓
Dynamic Analysis
   ↓
Impact Validation
```

**Firmware**

`v1.2.1 Build 20220715`

**Disclosure**

Vendor confirmed product **End-of-Life**.

</td>

<td width="33%" valign="top">

## 🏆 TikTok

### `$4,500 Responsible Disclosure Bounty`

<p>
<img src="https://img.shields.io/badge/Vulnerability_Research-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/Web_Security-111827?style=flat-square"/>
</p>

Identified and demonstrated a **high-impact security vulnerability**.

### Research Lifecycle

```text
DISCOVER
   ↓
VALIDATE
   ↓
PoC
   ↓
REPORT
   ↓
TRIAGE
   ↓
REMEDIATE
```

- Vulnerability discovery
- Full impact validation
- Sanitized proof of concept
- Technical report
- Coordinated triage
- Remediation verification

</td>

<td width="33%" valign="top">

## 📱 Coinbase Wallet

### `Android Security Research`

<p>
<img src="https://img.shields.io/badge/Android-111827?style=flat-square&logo=android"/>
<img src="https://img.shields.io/badge/AccessibilityService-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/BIP--39-111827?style=flat-square"/>
</p>

Research into sensitive-data exposure across Android accessibility boundaries.

### Focus

- BIP-39 seed phrase exposure
- `AccessibilityService`
- Controlled PoC APK
- Exfiltration testing
- Multi-device validation
- Mitigation analysis

Evaluated behavior around:

```java
importantForAccessibility=
    "no-hide-descendants"
```

and documented continued attack-surface behavior during follow-up testing.

</td>

</tr>
</table>

---

# 🔬 Firmware Research Methodology <sub><code>█</code></sub>

<div align="center">

```text
┌───────────────┐
│ Firmware Image│
└───────┬───────┘
        │
        ▼
┌───────────────┐
│   Extraction  │
│    Binwalk    │
└───────┬───────┘
        │
        ▼
┌────────────────────┐
│ Reverse Engineering│
│   Lua / LuCI / ASM │
└────────┬───────────┘
         │
         ▼
┌──────────────────┐
│  QEMU Emulation  │
│    ARM / MIPS    │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ Dynamic Analysis │
└────────┬─────────┘
         │
         ▼
┌──────────────────┐
│ Exploit Validation│
└────────┬─────────┘
         │
         ▼
┌───────────────────────┐
│ Responsible Disclosure│
└───────────────────────┘
```

</div>

---

# ⚡ Currently Building — <span style="color:#E11D48">LeakHunterX</span>

<table>
<tr>

<td width="50%" valign="top">

# 🔥 LeakHunterX

### Distributed Secret-Scanning Platform

**Founder @ TantraLogic AI**

LeakHunterX is a distributed secret-scanning SaaS designed to detect exposed credentials while keeping the user's source code **on their own machine**.

### Core Capabilities

- 🔐 Source code remains local
- 🔎 50+ secret detection patterns
- ⚡ Real-time distributed scanning
- 📊 JSON / CSV / PDF reporting
- 🔑 AWS, GitHub, Stripe, JWT & DB secret detection
- 🐳 Containerized infrastructure
- 🔌 Local agent architecture

<p>

<img src="https://img.shields.io/badge/50+_Patterns-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/<2%25_False_Positive-111827?style=flat-square"/>
<img src="https://img.shields.io/badge/Real--Time-111827?style=flat-square"/>

</p>

<a href="https://leakhunterx.com">
<img src="https://img.shields.io/badge/Visit_leakhunterx.com-E11D48?style=for-the-badge"/>
</a>

</td>

<td width="50%" valign="top">

## Architecture

```text
┌─────────────────────────┐
│   LOCAL SCANNER AGENT   │
│                         │
│  Source code stays here │
└────────────┬────────────┘
             │
             │ Token Authenticated
             │ WebSocket
             ▼
┌─────────────────────────┐
│      FastAPI Backend    │
└──────────┬───────┬──────┘
           │       │
           ▼       ▼
     ┌─────────┐ ┌────────────┐
     │  Redis  │ │ PostgreSQL │
     └────┬────┘ └─────┬──────┘
          │            │
          └──────┬─────┘
                 ▼
      ┌─────────────────────┐
      │ Real-Time Dashboard │
      │ Reports + Analytics │
      └─────────────────────┘
```

### Backend

`FastAPI` • `Redis` • `PostgreSQL`  
`WebSockets` • `SQLAlchemy` • `Docker`

</td>

</tr>
</table>

---

# 🚀 Featured Projects <sub><code>█</code></sub>

<table>
<tr>

<td width="25%" valign="top">

## 🧠 NYX

Open-source AI security research platform for:

- Attack-surface intelligence
- Dynamic analysis
- Vulnerability discovery
- Validation workflows

`Python` `AI` `Security`

<br/>

<a href="https://github.com/Omkar443/nyx">
<img src="https://img.shields.io/badge/View_Repository-E11D48?style=flat-square&logo=github"/>
</a>

</td>

<td width="25%" valign="top">

## 🛰️ ProbeRaptor

Modular reconnaissance framework for:

- Subdomain discovery
- CT log analysis
- Port scanning
- Target scoring

Built without third-party recon chaining.

`Python` `Recon`

<br/>

<a href="https://github.com/Omkar443/ProbeRaptor">
<img src="https://img.shields.io/badge/View_Repository-E11D48?style=flat-square&logo=github"/>
</a>

</td>

<td width="25%" valign="top">

## 🤖 LeakHunterX Agent

Autonomous security research agent for:

- Reconnaissance
- Attack-surface analysis
- Vulnerability discovery
- Research automation

`Python` `Agents`

<br/>

<a href="https://github.com/Omkar443/leakhunterx-agent">
<img src="https://img.shields.io/badge/View_Repository-E11D48?style=flat-square&logo=github"/>
</a>

</td>

<td width="25%" valign="top">

## ⚔️ Kioptrix Level 1

Technical exploitation walkthrough covering:

- Reconnaissance
- Enumeration
- Exploitation
- Privilege escalation

`Linux` `CTF`

<br/>

<a href="https://github.com/Omkar443/Kioptrix-Level1-Writeup">
<img src="https://img.shields.io/badge/View_Repository-E11D48?style=flat-square&logo=github"/>
</a>

</td>

</tr>
</table>

---

# ⚔️ Research Arsenal <sub><code>█</code></sub>

<table>

<tr>

<td width="25%" valign="top">

### 🔬 Security Research

`Firmware RE`

`Android`

`Web Security`

`API Security`

`IoT / Embedded`

`802.11 / RF`

</td>

<td width="25%" valign="top">

### 🛠 Security Tools

`Burp Suite`

`MobSF`

`JADX`

`Binwalk`

`QEMU`

`Metasploit`

`Nmap`

`Nessus`

`Kali Linux`

`NetHunter`

</td>

<td width="25%" valign="top">

### 💻 Languages

`Python`

`C`

`Java`

`JavaScript`

`SQL`

`MIPS Assembly`

`x86 Assembly`

</td>

<td width="25%" valign="top">

### ⚙️ Backend & Infra

`FastAPI`

`PostgreSQL`

`Redis`

`WebSockets`

`SQLAlchemy`

`Docker`

`Linux`

`Git`

</td>

</tr>

</table>

---

<table>
<tr>

<td width="33%" valign="top">

# ⚡ Hardware → Security

My **Electrical & Electronics Engineering** background gives me a hardware-level foundation for embedded and IoT research.

```text
Circuit Design
      │
      ▼
Digital Logic
      │
      ▼
Microprocessors
      │
      ▼
Assembly
      │
      ▼
Embedded Systems
      │
      ▼
Firmware RE
      │
      ▼
IoT Security
```

### Hardware Foundation

`Circuit Design`

`Microprocessor Architecture`

`Logic Gates`

`Assembly Language`

`ESP8266`

`Industrial Electrical Systems`

</td>

<td width="33%" valign="top">

# 🧭 My Journey

### `2018 → 2023`

**Diploma — Electrical & Electronics Engineering**

Korea Nepal Polytechnic Institute

↓

### `2023 → 2024`

**Sub Electrical Engineer**

Varun Beverages  
PepsiCo Franchise

↓

### `2024 → Present`

**B.Tech CSE — Cyber Security**

Parul University

↓

### `2025 → Present`

**Independent Security Research**

Firmware • Android • Web • IoT

↓

### `2025 → Present`

**Founder — LeakHunterX**

TantraLogic AI

</td>

<td width="33%" valign="top">

# 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Omkar443&show_icons=true&hide_border=true&bg_color=0D1117&title_color=E11D48&icon_color=E11D48&text_color=C9D1D9&ring_color=E11D48" width="100%"/>

<br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Omkar443&layout=compact&hide_border=true&bg_color=0D1117&title_color=E11D48&text_color=C9D1D9" width="100%"/>

</div>

</td>

</tr>
</table>

---

# 🎯 Current Focus

```bash
omkar@research:~$ cat focus.conf

[ RESEARCH ]
> Firmware Security
> Android Application Security
> IoT / Embedded Security
> Vulnerability Research

[ BUILDING ]
> LeakHunterX
> Security Automation
> Open-Source Research Tooling

[ INTERESTED_IN ]
> Firmware / Embedded Security
> Android Security
> Security Engineering
> Vulnerability Research
> Research Collaboration
```

---

# 📡 Connect <sub><code>█</code></sub>

<div align="center">

### Let's build a more secure digital world.

<br/>

<a href="https://leakhunterx.com">
<img src="https://img.shields.io/badge/🔥_LeakHunterX-E11D48?style=for-the-badge"/>
</a>

<a href="https://hackerone.com/omkar_sahni">
<img src="https://img.shields.io/badge/HackerOne-111827?style=for-the-badge&logo=hackerone&logoColor=white"/>
</a>

<a href="https://www.linkedin.com/in/omkar-sahni-89b952324">
<img src="https://img.shields.io/badge/LinkedIn-111827?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>

<a href="https://github.com/Omkar443">
<img src="https://img.shields.io/badge/GitHub-111827?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

```text
omkar@research:~$ ./find-next-bug

[+] loading research environment...
[+] vulnerabilities are everywhere...
[+] curiosity enabled...
[+] research never stops...

omkar@research:~$ █
```

<br/>

## `BREAK ASSUMPTIONS` <span style="color:#E11D48">//</span> `BUILD BETTER SYSTEMS`

<br/>

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&height=4&color=E11D48"/>

</div>
