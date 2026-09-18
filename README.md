<div align="center">

# Santiago López Castaño
### Cybersecurity · Web3 Security · Linux & Smart Contracts

**Available for hire** · Remote (CET) · Open to relocation

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/santiagolopez-cyber/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:santi.lpz28@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://santilpz28.github.io/chainguard-pages/)

</div>

---

## 👋 About me

I'm a cybersecurity analyst and Web3 security researcher with **5+ years** of professional experience spanning data analytics, system administration, and offensive security.

**Currently:** Data Analyst & Automation Specialist at **General Mills** (multinational F&B) — building Python pipelines, anomaly detection dashboards, and security automation.

**Previously:** Operations Supervisor in **Finland** (3 years) — managed international teams, built operational analytics, and worked in English in a multicultural Arctic environment.

**Certifications:** RHCSA (Red Hat, 2024) · eJPT (eLearnSecurity, 2025) · Microsoft Python (2023) · In progress: eWPT · Target: OSCP ~2026

**Master in Blockchain Development** (Solidity, Foundry, OpenZeppelin) — completed 2026.

I don't just write code. I **ship products that solve real problems**, document them well, and break them on purpose to make them stronger.

---

## 🎯 What I do

<table>
<tr>
<th>🔐 Offensive Security</th>
<th>⛓️ Web3 & Smart Contracts</th>
<th>🐧 Linux & DevSecOps</th>
</tr>
<tr>
<td>

- Network & Web Pentesting
- OWASP Top 10 exploitation
- Vulnerability assessment
- Burp Suite, Metasploit, Nmap
- Wireshark packet analysis
- CTF-style challenges

</td>
<td>

- Solidity smart contracts
- Foundry (forge, cast, fuzzing)
- Slither / Mythril static analysis
- EVM internals & gas optimization
- DeFi patterns (DEX, staking, escrow)
- Smart contract auditing

</td>
<td>

- RHCSA-certified Linux admin
- Docker & Docker Compose
- Bash & Python automation
- n8n workflow orchestration
- System hardening (SSH, iptables, UFW)
- Prometheus monitoring

</td>
</tr>
<tr>
<th>📊 Data & Automation</th>
<th>🌐 OSINT & Threat Intel</th>
<th>🛠️ Maker & IoT</th>
</tr>
<tr>
<td>

- Python (pandas, numpy)
- SQL (PostgreSQL, MySQL)
- Power BI / Tableau
- SAP cost control
- Anomaly detection on logs
- VBA / Excel automation

</td>
<td>

- Etherscan API integration
- VirusTotal, Shodan, Whois
- n8n domain risk scoring
- On-chain transaction tracing
- Phishing infrastructure mapping
- Domain reputation systems

</td>
<td>

- Raspberry Pi hardening
- ArduPilot / Pixhawk (drones)
- Flipper Zero + SDR research
- Nvidia Jetson (basic vision)
- MQTT infrastructure (Mosquitto)
- Local AI / LLM servers

</td>
</tr>
</table>

---

## 🚀 Featured Projects

### ⛓️ [ChainGuard.ai](https://github.com/santilpz28/cortex) — Web3 Risk Intelligence Platform
*2025 — present · Python, FastAPI, React, Docker, Prometheus*

A production-grade microservices platform that combines on-chain signals (Etherscan), repository metadata, and OSINT (VirusTotal, Shodan, Whois) into unified risk scores for Web3 domains, contracts, and addresses.

**Highlights:**
- 4 services: scraper, analysis, API, frontend
- TTL cache + rate limiting, SSRF hardening
- p99 ≤ 15s across the pipeline
- AI multi-model orchestrator (Hydra) with <200ms failover
- 186-entry crypto dictionary with 9 documented historical exploits
- Defense-in-depth: 3-layer whitelist (JS / PHP / Python)
- 34/34 security tests passing (including 15 injection attacks)
- Live deployment + audit reports

**Stack:** Python 3.10 (FastAPI, httpx, Pydantic Settings 2.0), React + Tailwind, Docker Compose, PostgreSQL, Prometheus.

[📂 Repo](https://github.com/santilpz28/cortex) · [🌐 Live demo](https://santilpz28.github.io/chainguard-pages/)

---

### ⛓️ [Solidity Security Labs](https://github.com/santilpz28/foundry-fundme-f25) — Foundry + Echidna
*2025 · Solidity, Foundry, OpenZeppelin, Echidna*

Hands-on labs covering smart contract security patterns: msg.sender vs tx.origin, custom errors, payable flows, CEI enforcement, access control, proxy/init guards, and upgradeable UUPS patterns.

- Foundry unit + fuzz tests
- Property-based testing with Echidna
- 90%+ test coverage on DeFi patterns (DEX router, staking, escrow)
- Auditing methodology: threat model → line-by-line review → report

[📂 Repo](https://github.com/santilpz28/foundry-fundme-f25)

---

### 🔐 [redops / Portly](https://github.com/santilpz28/port-scanner) — Network Recon Toolkit
*2024 — present · Python*

A multi-threaded port scanner with service detection, banner grabbing, and CSV export. Built for low-resource environments (VPS, IoT).

- Asyncio + threading hybrid
- Service fingerprinting
- Output formats: JSON, CSV, plain text
- Resilient to network jitter

[📂 Repo](https://github.com/santilpz28/port-scanner)

---

### 🌐 [n8n DomainScore Pipeline](https://github.com/santilpz28/cortex) — OSINT Orchestration
*2025 · n8n, VirusTotal, Shodan, Whois*

Workflow that scores domain risk in real time, penalizing:
- Malicious detections (VT > 0)
- Critical/non-standard open ports (Shodan)
- Young domains (< 90 days)

Productionized as the "domainScore" service in ChainGuard.

---

### 🚀 [orbital-shield](https://github.com/santilpz28/orbital-shield) — Space IoT Security Lab
*2025 · Python, Docker, MQTT/Mosquitto*

Experimental security framework for satellite IoT communications. Hardened MQTT broker + Python telemetry simulator.

- Mosquitto broker with TLS
- Message signing/verification
- Docker Compose for reproducible labs

[📂 Repo](https://github.com/santilpz28/orbital-shield)

---

### 🤖 [ai-soberana](https://github.com/santilpz28/ai-soberana) — Local AI Server
*2025 · Python, Docker, OpenAI-compatible API*

Self-hosted LLM inference stack with privacy-first design. Run models locally, no cloud, full data sovereignty.

[📂 Repo](https://github.com/santilpz28/ai-soberana)

---

## 📚 Write-ups & CTF

### Featured CTF Writeups

Technical writeups with production parallels, published via [chainguard-pages](https://santilpz28.github.io/chainguard-pages/#writeups).

#### NavajaNegra 2025 — Caliphal Labs CTF

| Challenge | Class | Vulnerability | Writeup |
|---|---|---|---|
| **MD5 Road** | Crypto | Truncated MD5 prefix collision (20-bit comparison) — birthday attack | [read →](https://santilpz28.github.io/chainguard-pages/writeups/ctf-md5-truncated-collision.html) |
| **Space Pinch** | Side-channel | Reed-Solomon multi-sample majority-vote attack (32 noisy queries) | [read →](https://santilpz28.github.io/chainguard-pages/writeups/ctf-reed-solomon-multisample.html) |

#### Hackademics Forum CTF 2025 — Daysa

| Challenge | Class | Vulnerability | Writeup |
|---|---|---|---|
| **MD5 Road — The Revenge** | Crypto | The server hands you `md5(secret)` in the banner. Send the MD5 internal padding as your input and the server turns into a length-extension oracle. Byte-by-byte recovery of the 52-byte secret in about 13K hash predictions. | [read →](https://santilpz28.github.io/chainguard-pages/writeups/ctf-md5-length-extension-revenge.html) |

### Other CTF & learning repos

| Resource | Description |
|---|---|
| [Ethernaut Solutions (Foundry)](https://github.com/santilpz28/ethernaut-foundry) | Solve Ethernaut CTF levels using Foundry |
| [Damn Vulnerable DeFi](https://github.com/santilpz28/dvdf-solutions) | Walkthroughs of DeFi exploits |
| [HackTheBox Write-ups](https://github.com/santilpz28/htb-writeups) | Selected retired machines, focus on web + AD |
| [Master Signature Attacks](https://github.com/santilpz28/master-signature-attacks) | Solidity security workshop: vulnerable vs secure `ecrecover` |
| [RedOps Toolkit](https://github.com/santilpz28/redops) | Red Team toolkit — port scanning, recon, wordlists, exploits |

---

## 📊 GitHub Stats

<div align="center">

![Profile views](https://komarev.com/ghpvc/?username=santilpz28&color=blueviolet&style=flat-square)
![GitHub followers](https://img.shields.io/github/followers/santilpz28?style=social)

</div>

---

## 🌍 Languages

- **Spanish:** Native
- **English:** C1 (Advanced) — *3 years working full-time in English (Finland)*
- **Russian:** Intermediate

---

## 📫 How to reach me

- **Email:** santi.lpz28@gmail.com
- **LinkedIn:** [/in/santiagolopez-cyber](https://www.linkedin.com/in/santiagolopez-cyber/)
- **Portfolio:** [santilpz28.github.io/chainguard-pages](https://santilpz28.github.io/chainguard-pages/)
- **Phone:** +34 613 20 6565

> *Open to roles in Cybersecurity, Web3 Security (Solidity auditing), and Linux/DevSecOps.*
> *Remote-first (CET), but open to relocation in EU and Switzerland.*
> *Available for short-term contracts and long-term engagements.*

---

<div align="center">

**Built with discipline. Audited with rigor. Documented with care.**

⚡ *"If you can't break it, you don't own it."* ⚡

</div>
