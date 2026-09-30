# Awesome-Continuous-Threat-Exposure-Management

# Top Continuous Threat Exposure Management (CTEM) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Exposure Assessment, Attack Path Validation, Risk-Based Prioritization & Remediation Orchestration*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Continuous Threat Exposure Management (CTEM)**. These tools help security teams continuously discover, validate, prioritize, and remediate exposures across hybrid environments—moving beyond static vulnerability scoring to actionable, threat-informed risk reduction.

**Examples** include XM Cyber, Picus Security, Cymulate, Tenable ExposureAI, SafeBreach, AttackIQ, Palo Alto Exposure Management, Qualys TruRisk, Rapid7 Exposure Command, and Kenna Security (the category leaders).

**Open-source emphasis**: CTEM has a **small but emerging open-source ecosystem**. The most complete platform is **ExposureNexus**, an early-stage CTEM platform for importing scanner findings and tracking triage through remediation . **OpenBAS** (Open Breach and Attack Simulation) provides 639 stars and is the leading open-source BAS platform . **MITRE Caldera** is the default open-source adversary emulation framework for purple-team exercises . **VMC** (OWASP) delivers asset-aware, CVSS-driven vulnerability prioritization . This section documents these focused solutions honestly.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[XM Cyber](https://xmcyber.com/)**
  Continuous threat exposure management platform focused on attack path analysis. Maps potential attack routes across hybrid environments and prioritizes remediation based on critical asset reachability.

- **[Picus Security](https://www.picussecurity.com/)**
  Security validation platform that continuously tests, measures, and optimizes security controls against real-world attack techniques. Provides BAS capabilities integrated with exposure management.

- **[Cymulate](https://cymulate.com/)**
  Breach and attack simulation platform that validates security controls and identifies exposure gaps through continuous automated testing.

- **[Tenable ExposureAI](https://www.tenable.com/)**
  AI-powered exposure management platform providing unified visibility across IT, cloud, and OT environments. Uses AI and machine learning for threat detection, data exposure detection, and prompt translation to identify security gaps .

- **[SafeBreach](https://www.safebreach.com/)**
  Continuous security validation platform with breach and attack simulation. Provides automated attack simulation across the kill chain to validate security controls.

- **[AttackIQ](https://www.attackiq.com/)**
  Breach and attack simulation platform that continuously validates security controls against MITRE ATT&CK techniques.

- **[Palo Alto Exposure Management](https://www.paloaltonetworks.com/)**
  Exposure management capabilities within Cortex XDR and Prisma Cloud. Integrates third-party scanner data for unified risk prioritization .

- **[Qualys TruRisk](https://www.qualys.com/)**
  Qualys Enterprise TruRisk Management (ETM) platform providing cloud-based Risk Operations Center. Uses TruRisk 2.0 scoring with maximum detection score approach, CVE standardization, and 25+ threat intelligence sources. Features TruLens for peer benchmarking, WOW/AWE/REG exposure timing metrics, and 40-day early KEV warning .

- **[Rapid7 Exposure Command](https://www.rapid7.com/)**
  Exposure management platform providing unified attack surface visibility with 290+ integrations. Features **runtime validation** via eBPF sensors, **DSPM** for data-aware risk prioritization, and **Remediation Hub** with 550+ prebuilt workflows. Named a Leader in 2025 IDC MarketScape and 2025 Gartner Magic Quadrant .

- **[Kenna Security (Cisco)](https://www.kennasecurity.com/)**
  Risk-based vulnerability management platform acquired by Cisco. Pioneered risk-based prioritization with real-time threat and exploit intelligence. Protects 14M+ assets and manages 12.7B+ vulnerabilities. Integration with Cisco SecureX for orchestration .

## Open-Source GitHub Projects

### CTEM Platforms

- **[ExposureNexus](https://github.com/s-schoen/exposurenexus)**
  **The most complete open-source CTEM platform.** Early development stage. Imports **Nuclei JSONL** findings and normalizes them into a core model of **Assets, Vulnerabilities, and Findings** . Provides a **triage queue** grouped around affected assets, tracks finding status from discovery through confirmation, mitigation, accepted risk, false positive, duplicate, or out-of-scope. Features assignment, due dates, asset inventory management, vulnerability catalog browsing, and role-based access control (viewer, editor, admin). Docker Compose deployment with PostgreSQL .

### Breach & Attack Simulation

- **[OpenBAS](https://github.com/OpenBAS-Platform/openbas)**
  **The leading open-source Breach and Attack Simulation platform.** **639 stars, 68 forks**, Java-based. Provides automated attack simulation to validate security controls and identify exposure gaps .

- **[MITRE Caldera](https://github.com/mitre/caldera)**
  **The default open-source adversary emulation framework.** Automates ATT&CK technique execution against target environments via lightweight agents. Ships with ready-made adversary profiles (APT29, ransomware chains) for purple-team exercises, SIEM detection validation, and EDR coverage testing. Free, ATT&CK-native, and scriptable .

### Vulnerability Prioritization

- **[VMC (Vulnerability Management Center)](https://github.com/OWASP/VMC)**
  **OWASP-hosted open-source platform for asset-aware vulnerability prioritization.** Ingests Nessus/OpenVAS reports, matches with asset inventory, and **recomputes CVSS v2/v3 environmental scores** asynchronously. Integrates with **TheHive** for case management. Docker Compose, Apache-2.0. Supports peer-reviewed CVSS studies .

- **[OpenASM](https://github.com/oasm-platform/open-asm)**
  **AI-powered open-source Attack Surface Management platform.** Discovers and manages internet-facing assets, performs vulnerability assessment, and provides **MCP server for AI assistant integration** (OpenAI, Anthropic, Google) to query asset data via natural language. Distributed scanning engine with pluggable connectors (nuclei, subfinder, httpx, naabu, dnsx). Multi-workspace, S3-compatible storage, Slack/Telegram/Webhook integrations .

### Threat Intelligence

- **[OpenCTI](https://github.com/OpenCTI-Platform/opencti)**
  **Leading open-source threat intelligence platform from Filigran.** Structures and operationalizes holistic threat intelligence across technical, operational, and strategic levels. Enables security teams to contextualize attacks and act proactively. Foundation for **threat-informed CTEM** .

- **[Filigran OpenAEV](https://github.com/OpenAEV-Platform/openaev)**
  Open-source platform for **attack simulation, resilience testing, and crisis management exercises**. Part of Filigran's open-source CTEM suite alongside OpenCTI .

### Additional Strong Open-Source Options

- **CTEM Platform**: **ExposureNexus** (Nuclei import, triage workflow) .
- **Breach & Attack Simulation**: **OpenBAS** (639 stars, Java), **MITRE Caldera** (ATT&CK-native, default choice) .
- **Vulnerability Prioritization**: **VMC** (OWASP, CVSS environmental scores, TheHive integration) .
- **Attack Surface Management**: **OpenASM** (AI-powered, MCP integration) .
- **Threat Intelligence**: **OpenCTI** (Filigran, threat-informed CTEM), **OpenAEV** (attack simulation) .

**Frameworks for building custom systems**: Combine **ExposureNexus** for CTEM triage workflow, **OpenBAS** or **MITRE Caldera** for breach and attack simulation, **VMC** for CVSS-driven prioritization, **OpenASM** for attack surface discovery, and **OpenCTI** for threat intelligence enrichment. Add **PostgreSQL** for persistence and **TheHive** for case management.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- CTEM platforms handle sensitive security and vulnerability data; ensure proper access controls and compliance with organizational security policies.
- **Open-source reality**: The open-source ecosystem for CTEM is **emerging but not yet equivalent to commercial platforms**. **ExposureNexus** provides a CTEM triage foundation but is early-stage . **OpenBAS** and **MITRE Caldera** deliver production-grade breach and attack simulation . **VMC** offers rigorous CVSS-driven prioritization . **OpenASM** provides AI-powered attack surface discovery . However, **commercial platforms** (XM Cyber, Rapid7 Exposure Command, Qualys TruRisk, Tenable ExposureAI) provide **unified attack path analysis, runtime validation, automated remediation, and enterprise-scale orchestration** that open-source alternatives require significant assembly and engineering investment to match.

---

**Made for security engineers, vulnerability management teams, SOC analysts, and exposure management practitioners.**
Let's make continuous threat exposure management more open, transparent, and actionable.
