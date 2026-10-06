<!-- =========================================================
     OMKAR443 — GITHUB PROFILE README
     Security Researcher • Firmware RE • Android • Web • IoT
========================================================== -->

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,55:111827,100:7F1D1D&height=220&section=header&text=OMKAR%20SAHNI&fontSize=48&fontColor=F8FAFC&fontAlignY=36&desc=SECURITY%20RESEARCHER%20%2F%2F%20VULNERABILITY%20RESEARCHER&descAlignY=56&descSize=16&animation=fadeIn" />

### `FIRMWARE RE` • `ANDROID SECURITY` • `WEB SECURITY` • `IoT`

<br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2600&pause=900&color=F43F5E&center=true&vCenter=true&width=700&lines=Firmware+Reverse+Engineering;Android+Security+Research;Vulnerability+Research;Building+LeakHunterX;Breaking+assumptions.+Building+security." alt="Typing SVG" />

<br>

> **Reverse engineering systems. Breaking assumptions. Building security tooling.**

<br>

<a href="https://leakhunterx.com">
  <img src="https://img.shields.io/badge/LeakHunterX-Visit-111827?style=for-the-badge&logo=securityscorecard&logoColor=white&labelColor=7F1D1D" />
</a>
<a href="https://hackerone.com/omkar_sahni">
  <img src="https://img.shields.io/badge/HackerOne-Profile-111827?style=for-the-badge&logo=hackerone&logoColor=white&labelColor=7F1D1D" />
</a>
<a href="https://www.linkedin.com/in/omkar-sahni-89b952324">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-111827?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=7F1D1D" />
</a>

</div>

---

## `$ whoami`

```bash
omkar@research:~$ whoami

Security Researcher
Vulnerability Researcher
Firmware Reverse Engineer
Security Tool Builder
Founder @ LeakHunterX
```

I am an independent security researcher focused on **firmware reverse engineering, Android security, vulnerability research, IoT security, and offensive security engineering**.

My work spans the full vulnerability research lifecycle:

```text
RECON → STATIC ANALYSIS → REVERSE ENGINEERING → EMULATION
           ↓
DISCLOSURE ← VALIDATION ← EXPLOIT RESEARCH ← DYNAMIC ANALYSIS
```

I also build security infrastructure and automation, including **LeakHunterX**, a distributed secret-scanning platform designed to analyze source code while keeping customer source files local.

<br>

```text
[+] Firmware Reverse Engineering     ARM / MIPS
[+] Android Application Security     IPC / Intents / Accessibility
[+] Web & API Security               Offensive Research
[+] IoT / Embedded Security          Hardware + Firmware
[+] Security Automation              Python / Backend Systems
[+] Vulnerability Research           PoC → Disclosure → Verification
```

---

# 🛡️ Selected Security Research

<table>
<tr>
<td width="33%" valign="top">

### 📡 TP-Link Archer C7 v5

**2 CVE submissions pending with MITRE**

`Firmware RE` `ARM` `QEMU` `Binwalk`

Full firmware research chain covering extraction, reverse engineering, emulation and dynamic analysis.

**Research findings**

**CWE-78**  
Command injection in a LuCI web-interface handler with root-level code-execution impact.

**CWE-321**  
Hardcoded RSA private-key material recovered from distributed firmware.

**Firmware**

`v1.2.1 Build 20220715`

**Disclosure**

Vendor confirmed the affected product as End-of-Life.

</td>

<td width="33%" valign="top">

### 🏆 TikTok

**$4,500 Responsible Disclosure Bounty**

Identified and demonstrated a high-impact security vulnerability.

Research involved:

- Vulnerability discovery
- Impact validation
- Sanitized proof of concept
- Technical reporting
- Coordinated triage
- Remediation verification

```text
DISCOVER
   ↓
VALIDATE
   ↓
REPORT
   ↓
TRIAGE
   ↓
REMEDIATE
```

</td>

<td width="33%" valign="top">

### 📱 Coinbase Wallet

**Android Security Research**

Research into sensitive data exposure across Android accessibility boundaries.

Focus areas:

- BIP-39 seed phrase exposure
- `AccessibilityService`
- Controlled PoC APK
- Multi-device validation
- Exfiltration testing
- Mitigation analysis

Evaluated behavior around:

`importantForAccessibility="no-hide-descendants"`

</td>
</tr>
</table>

---

## 🔬 Firmware Research Methodology

```mermaid
flowchart LR
    A[Firmware Image] --> B[Extraction]
    B --> C[Filesystem Analysis]
    C --> D[Reverse Engineering]
    D --> E[QEMU Emulation]
    E --> F[Dynamic Analysis]
    F --> G[Impact Validation]
    G --> H[Responsible Disclosure]
```

```text
Tools commonly involved:

Binwalk
   ↓
Filesystem / Lua / LuCI
   ↓
ARM / MIPS Analysis
   ↓
QEMU
   ↓
Dynamic Testing
   ↓
Exploit Validation
```

---

# ⚡ Currently Building

<div align="center">

## `LeakHunterX`

### Distributed Secret-Scanning Infrastructure

**Founder @ TantraLogic AI**

<a href="https://leakhunterx.com">
<img src="https://img.shields.io/badge/LEAKHUNTERX-VISIT_PLATFORM-E11D48?style=for-the-badge&labelColor=111827" />
</a>

</div>

LeakHunterX is a distributed secret-scanning platform designed to detect exposed credentials while keeping the user's source code on their own machine.

### Architecture

```mermaid
flowchart LR
    A[Local Scanner Agent] -->|Token Authenticated WebSocket| B[FastAPI Backend]
    B --> C[(Redis)]
    B --> D[(PostgreSQL)]
    B --> E[Real-Time Dashboard]
    E --> F[JSON / CSV / PDF Reports]

    A -. Source code remains local .-> A
```

### Highlights

```text
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  🔐 Source code remains on the user's machine              │
│                                                             │
│  🔎 50+ secret detection patterns                          │
│                                                             │
│  ⚡ Real-time distributed scanning                         │
│                                                             │
│  🧠 Credential & secret classification                     │
│                                                             │
│  📊 JSON / CSV / PDF reporting                            │
│                                                             │
│  🐳 Containerized backend architecture                    │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

Detection includes patterns associated with:

`AWS` • `GitHub` • `Stripe` • `JWT` • `Database URIs` • `API Keys` • `Credentials`

---

# 🚀 Featured Security Projects

<table>
<tr>

<td width="50%" valign="top">

## 🧠 NYX

**AI Security Research Platform**

Open-source security research platform combining:

- AI security agents
- Attack-surface intelligence
- Dynamic analysis
- Vulnerability discovery
- Validation workflows
- Security knowledge automation

**Primary language:** `Python`

<a href="https://github.com/Omkar443/nyx">
<img src="https://img.shields.io/badge/VIEW-NYX-E11D48?style=flat-square&logo=github&logoColor=white" />
</a>

</td>

<td width="50%" valign="top">

## 🛰️ ProbeRaptor

**Reconnaissance Framework**

Original Python reconnaissance suite designed for bug-bounty attack-surface discovery.

Capabilities include:

- Subdomain brute forcing
- Certificate Transparency analysis
- Parallel port scanning
- Target scoring
- JSON reporting

Built without chaining third-party reconnaissance tools.

<a href="https://github.com/Omkar443/ProbeRaptor">
<img src="https://img.shields.io/badge/VIEW-PROBERAPTOR-E11D48?style=flat-square&logo=github&logoColor=white" />
</a>

</td>
</tr>

<tr>

<td width="50%" valign="top">

## 🤖 LeakHunterX Agent

**Autonomous Security Research Agent**

Security research agent focused on:

- Reconnaissance
- Attack-surface analysis
- Vulnerability discovery
- Research automation

**Primary language:** `Python`

<a href="https://github.com/Omkar443/leakhunterx-agent">
<img src="https://img.shields.io/badge/VIEW-LHX_AGENT-E11D48?style=flat-square&logo=github&logoColor=white" />
</a>

</td>

<td width="50%" valign="top">

## ⚔️ Kioptrix Level 1

**Exploitation Research / Write-up**

Technical walkthrough covering:

- Reconnaissance
- Service enumeration
- Exploitation
- Linux privilege escalation
- Root access

<a href="https://github.com/Omkar443/Kioptrix-Level1-Writeup">
<img src="https://img.shields.io/badge/VIEW-WRITEUP-E11D48?style=flat-square&logo=github&logoColor=white" />
</a>

</td>

</tr>
</table>

---

# ⚔️ Research Arsenal

### Security Research

<p>
<img src="https://img.shields.io/badge/Firmware_RE-111827?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/Android_Security-111827?style=flat-square&logo=android&logoColor=white" />
<img src="https://img.shields.io/badge/Web_Security-111827?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/API_Security-111827?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/IoT_Security-111827?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/802.11_RF-111827?style=flat-square&logoColor=white" />
</p>

### Security Tooling

<p>
<img src="https://img.shields.io/badge/Burp_Suite-111827?style=flat-square&logo=burpsuite&logoColor=FF6633" />
<img src="https://img.shields.io/badge/MobSF-111827?style=flat-square" />
<img src="https://img.shields.io/badge/JADX-111827?style=flat-square" />
<img src="https://img.shields.io/badge/Binwalk-111827?style=flat-square" />
<img src="https://img.shields.io/badge/QEMU-111827?style=flat-square&logo=qemu&logoColor=white" />
<img src="https://img.shields.io/badge/Metasploit-111827?style=flat-square&logo=metasploit&logoColor=white" />
<img src="https://img.shields.io/badge/Nmap-111827?style=flat-square" />
<img src="https://img.shields.io/badge/Nessus-111827?style=flat-square" />
<img src="https://img.shields.io/badge/Kali_Linux-111827?style=flat-square&logo=kalilinux&logoColor=white" />
</p>

### Languages

<p>
<img src="https://img.shields.io/badge/Python-111827?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/C-111827?style=flat-square&logo=c&logoColor=white" />
<img src="https://img.shields.io/badge/Java-111827?style=flat-square&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-111827?style=flat-square&logo=javascript&logoColor=white" />
<img src="https://img.shields.io/badge/SQL-111827?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/MIPS_Assembly-111827?style=flat-square" />
<img src="https://img.shields.io/badge/x86_Assembly-111827?style=flat-square" />
</p>

### Backend & Infrastructure

<p>
<img src="https://img.shields.io/badge/FastAPI-111827?style=flat-square&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-111827?style=flat-square&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-111827?style=flat-square&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/WebSockets-111827?style=flat-square" />
<img src="https://img.shields.io/badge/SQLAlchemy-111827?style=flat-square" />
<img src="https://img.shields.io/badge/Docker-111827?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-111827?style=flat-square&logo=linux&logoColor=white" />
<img src="https://img.shields.io/badge/Git-111827?style=flat-square&logo=git&logoColor=white" />
</p>

---

# ⚡ Hardware → Security

My route into cybersecurity started with **Electrical & Electronics Engineering**.

That background gave me a foundation in:

```text
Circuit Design
     │
     ▼
Digital Logic
     │
     ▼
Microprocessor Architecture
     │
     ▼
Assembly Language
     │
     ▼
Embedded Systems
     │
     ▼
Firmware Reverse Engineering
     │
     ▼
IoT Security
```

This hardware perspective directly influences the way I approach embedded and firmware security research.

---

# 🧭 Journey

```mermaid
flowchart LR

    A[Electrical & Electronics Engineering] --> B[Industrial Electrical Engineering]
    B --> C[Computer Science + Cybersecurity]
    C --> D[Vulnerability Research]
    D --> E[Firmware + Android Security]
    E --> F[LeakHunterX]

```

### `2018 → 2023`

**Diploma — Electrical & Electronics Engineering**

Korea Nepal Polytechnic Institute

`Microprocessors` • `Assembly` • `Circuit Design` • `Digital Logic`

### `2023 → 2024`

**Sub Electrical Engineer**

Varun Beverages — PepsiCo Franchise

Worked with industrial electrical systems, maintenance and hardware fault diagnosis.

### `2024 → Present`

**B.Tech — Computer Science Engineering (Cyber Security)**

Parul University

### `2025 → Present`

**Independent Security Research**

`Firmware` • `Android` • `Web` • `IoT`

### `2025 → Present`

**Founder — LeakHunterX / TantraLogic AI**

Building security infrastructure and automated vulnerability-research tooling.

---

# 📊 GitHub Activity

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Omkar443&show_icons=true&hide_border=true&bg_color=0D1117&title_color=F43F5E&icon_color=F43F5E&text_color=C9D1D9&ring_color=F43F5E" />

<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Omkar443&layout=compact&hide_border=true&bg_color=0D1117&title_color=F43F5E&text_color=C9D1D9" />

</div>

---

# 🔭 Current Focus

```text
[ RESEARCH ]

Firmware Security
Android Application Security
IoT / Embedded Security
Vulnerability Research


[ BUILDING ]

LeakHunterX
Security Research Automation
Open-Source Security Tooling


[ INTERESTED IN ]

Firmware / Embedded Security
Android Security
Security Engineering
Vulnerability Research
Research Collaboration
```

---

# 📡 Connect

<div align="center">

<a href="https://leakhunterx.com">
<img src="https://img.shields.io/badge/LeakHunterX-E11D48?style=for-the-badge&logo=firefoxbrowser&logoColor=white" />
</a>

<a href="https://hackerone.com/omkar_sahni">
<img src="https://img.shields.io/badge/HackerOne-111827?style=for-the-badge&logo=hackerone&logoColor=white" />
</a>

<a href="https://www.linkedin.com/in/omkar-sahni-89b952324">
<img src="https://img.shields.io/badge/LinkedIn-111827?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>

<a href="https://github.com/Omkar443">
<img src="https://img.shields.io/badge/GitHub-111827?style=for-the-badge&logo=github&logoColor=white" />
</a>

</div>

<br>

<div align="center">

```text
omkar@research:~$ ./find-next-bug

[+] loading research environment...
[+] initializing toolchain...
[+] attack surface identified...
[+] curiosity enabled...

research never stops.

█
```

<br>

### `BREAK ASSUMPTIONS // BUILD BETTER SYSTEMS`

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,55:111827,100:7F1D1D&height=120&section=footer" />

</div>
