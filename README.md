<div align="center">

# Santiago López Castaño

**Cybersecurity & Automation Engineer · Offensive Security & Web3 Security**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/santiagolopez-cyber/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:santi.lpz28@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://santilpz28.github.io/chainguard-pages/)

</div>

---

## Profile

Cybersecurity & Automation Engineer with 2+ years of enterprise automation at **General Mills** (Python RPA, SAP data pipelines, RBAC cloud migration) and hands-on offensive security: Linux hardening, container security, and smart contract auditing.

- **eJPT** certified (Junior Penetration Tester) · **OSCP** in progress
- Speaker at **Hack-én 2026** on Web3 vulnerabilities
- 2nd place, global cybersecurity hackathon (50+ teams)

---

## Experience

**General Mills** — Data Architecture & Automation · San Adrián, Spain · *Oct 2024 – Present*
- Cut financial reporting from **5 hours → 40 minutes (−86%)** with a Python RPA script automating data migration into SAP, removing manual entry errors.
- Migrated Excel-based workflows to a centralized cloud environment with **RBAC**, improving cross-team productivity by 30%.
- Designed a scalable database architecture for automated analytics: report generation **2 hours → 5 minutes (−95%)**, with data integrity and reliable execution.

**Chain-Cortex** (Open Source) — Builder & Project Lead · Remote · *Jan 2026 – Present*
- **Agentic AI & Threat Intel (Hydra):** multi-model LLM orchestrator (OpenAI, Anthropic, Groq/Gemini fallback, local models) with majority voting, correlating OSINT feeds (Shodan, VirusTotal, Whois) to automate vulnerability triage, honeypot detection, and malicious node analysis.
- **Offensive Tooling & Auditing (ChainGuard):** 4-service Docker platform (Python, FastAPI, Prometheus) for continuous vulnerability scanning; audited DeFi/ERC-20 contracts with Solidity + Foundry (**120+ tests**), flagging **12+ exploit vectors** (reentrancy, access control).
- **Linux & Container Hardening:** secured production Ubuntu VPS nodes and container workloads with read-only filesystems, capability drops, non-root execution, UFW/Fail2ban rules, and Zero-Trust SSH control channels.

**Wild About Lapland** — Operations & Customer Supervisor · Rovaniemi, Finland · *Oct 2021 – May 2024*
- Ran daily operations, vendor scheduling, and incident response for **1,000+ international clients** per season, maintaining a **4.7/5** customer satisfaction score.
- Replaced manual, ad-hoc organization with a central database and standard operating procedures.

---

## Projects

### ⛓️ [ChainGuard](https://github.com/santilpz28/cortex) — Web3 Risk Intelligence Platform
*Python, FastAPI, React, Docker, PostgreSQL, Prometheus*

Multi-chain risk scoring platform combining on-chain signals (Etherscan, Solscan), repository metadata, and OSINT (VirusTotal, Shodan, Whois) into unified risk scores for domains, contracts, and addresses.

- 4 services: scraper, analysis, API, frontend · TTL cache, rate limiting, SSRF hardening
- **34/34 security tests passing** (15 explicit injection attacks: SQLi, XSS, SSTI, command injection, path traversal)
- 186-entry crypto dictionary across 5 chains with 9 documented historical exploits
- Hydra multi-model orchestrator with <200ms failover · EIP-712 wallet auth

[Repo](https://github.com/santilpz28/cortex) · [Live demo](https://santilpz28.github.io/chainguard-pages/)

### 🔐 [PHP2Shell](https://github.com/santilpz28/php2shell-pub) — CVE-2026-109618 / CVE-2026-109619 Research
*Python, Docker, PHP internals · CVSS v4.0 9.2 (Critical)*

Anatomy of two critical PHP core CVEs: a use-after-free in the session layer reaching RCE without authentication. Published with a working differential detector and verified backport of the official patch.

- Behavioural diff engine detecting the UAF **without** offsets or ASLR reliance
- 3 local Docker targets: vulnerable 8.2.34, patched 8.2.35, and 8.2.34 + backported patch (same version string)
- **6/6 UAF reproduced** on unpatched, **0/6** on patched, measured on a real binary
- Analysis cross-checked against advisory `GHSA-6wmf-4rv5-p3rp`

[Repo (ES)](https://github.com/santilpz28/php2shell-pub) · [Repo (EN)](https://github.com/santilpz28/php2shell-pub-en)

### 🤖 [JARVIS](https://github.com/santilpz28) — Self-Hosted AI Security Agent
*Python, Linux, Docker, LLM orchestration*

Self-hosted AI agent running local LLMs to keep code-audit data off third-party clouds, connected to a hardened Linux VPS over an encrypted Zero-Trust tunnel.

### 🔧 [redops](https://github.com/santilpz28/redops) — Network Recon Toolkit
*Python, asyncio + threading*

Small, auditable CLI tools for offensive security — each does one thing, no obfuscation, <200 LOC per tool.

| Tool | Function |
|---|---|
| `portly` | Multi-threaded port scanner — CIDR ranges, banner grab, JSON/CSV output |
| `subrecon` | Subdomain enumerator — crt.sh, wordlist, VirusTotal |
| `dirbust` | Web directory buster — status-code triage |

[Repo](https://github.com/santilpz28/redops)

### ⛓️ Solidity Security Labs — Foundry
*Solidity, Foundry, OpenZeppelin*

DeFi protocol implementations built from scratch with full test suites:

| Project | Scope | Tests |
|---|---|---|
| [master-lending-protocol](https://github.com/santilpz28/master-lending-protocol) | Non-custodial lending — collateral management, EIP-712 gasless auth, liquidations | 43/43 |
| [master-dao-governance](https://github.com/santilpz28/master-dao-governance) | On-chain DAO — proposal lifecycle, voting, quorum, treasury | 27/27 |
| [master-staking-and-nft](https://github.com/santilpz28/master-staking-and-nft) | Fixed-amount staking pool + peer-to-peer NFT marketplace | 24/24 |
| [master-yield-farming](https://github.com/santilpz28/master-yield-farming) | Multi-pool yield farming with `abi.encodePacked` optimizations | 14/14 |
| [foundry-fundme-f25](https://github.com/santilpz28/foundry-fundme-f25) | Security labs — `msg.sender` vs `tx.origin`, CEI, UUPS proxies | — |
| [ethernaut-foundry](https://github.com/santilpz28/ethernaut-foundry) | Ethernaut CTF levels solved in Foundry | — |

### 🏠 [home-lab](https://github.com/santilpz28/home-lab) — Hardware & IoT Security
*Embedded Linux, Raspberry Pi, MQTT, SDR*

Personal lab for embedded security research: Raspberry Pi 4B hardening, Pixhawk drone telemetry, Flipper Zero, MQTT/TLS messaging, local AI inference.

---

## Security Research & Write-ups

**[Portfolio write-ups](https://santilpz28.github.io/chainguard-pages/#writeups)**

- **The Graph Protocol** — Independent two-axis audit, score **8.2/10**, 0 critical, 10 findings across 1,606 raw Slither reports.
- **NavajaNegra 2025 (Caliphal Labs)** — MD5 truncated collision (5-char prefix brute-force) · Reed-Solomon multi-sample recovery.
- **Hackademics Forum CTF 2025 (Daysa)** — MD5 length-extension attack recovering a 52-byte secret in ~13K hash predictions.

---

## Skills

| Area | Stack |
|---|---|
| **Offensive security** | Pentesting, OWASP Top 10 exploitation, vulnerability assessment, Burp Suite, Nmap, Wireshark |
| **Web3 / Smart contracts** | Solidity, Foundry, OpenZeppelin, Slither, EIP-712, DeFi (lending, staking, DAO, yield farming), ERC-20/721 |
| **Linux & DevSecOps** | Ubuntu/RHEL, Docker, Kubernetes, Terraform, UFW/Fail2ban, SSH hardening, Prometheus |
| **Automation & Data** | Python (FastAPI, pandas), SQL (PostgreSQL, MySQL), SAP, RPA, RBAC |
| **OSINT & Threat intel** | VirusTotal, Shodan, Whois, Etherscan, on-chain tracing, n8n orchestration |
| **Cloud & AI** | AWS, self-hosted LLM inference, multi-model orchestration |

---

## Education

**Higher Technician in IT Systems & Networks (ASIR)** — Cybersecurity specialization · The Power, Remote · *Sept 2024 – Jun 2026*

**Ethereum Development & Web3 Security Intensive** — Blockchain Accelerator, Remote · *Sept 2025 – May 2026*

**Bachelor's in Business Administration** — Loyola Andalucía, Córdoba · *2017 – 2021*
Erasmus Exchange — Lapland AMK, Rovaniemi, Finland · *Jan – May 2021*

---

## Certifications

**eJPT** — Junior Penetration Tester (eLearnSecurity) · **OSCP** — in progress

---

## Contact

- **Email:** santi.lpz28@gmail.com
- **LinkedIn:** [/in/santiagolopez-cyber](https://www.linkedin.com/in/santiagolopez-cyber/)
- **Portfolio:** [santilpz28.github.io/chainguard-pages](https://santilpz28.github.io/chainguard-pages/)
- **Phone:** +34 613 20 6565

**Languages:** Spanish (native) · English (C1) · Russian (A2)

---

<div align="center">

![Profile views](https://komarev.com/ghpvc/?username=santilpz28&color=blueviolet&style=flat-square)

*Available for Cybersecurity, Web3 Security (Solidity auditing), and Linux/DevSecOps roles — remote-first (CET), open to EU/Switzerland relocation.*

</div>
