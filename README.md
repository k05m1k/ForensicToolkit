# 🛡️ Complete Forensic Toolkit v2

## Overview
Complete Forensic Toolkit v2 is a modular, professional-grade threat hunting and incident response toolkit built to empower SOC teams working in Microsoft Defender, Sentinel, and integrated SOAR ecosystems. It includes telemetry queries, email and IOC enrichment tools, persistence detection methods, memory and disk analysis workflows, and executive reporting templates.

---

## 🔍 Features
- Microsoft Defender & Sentinel-compatible KQL scripts
- Python tooling for phishing email parsing and IOC enrichment
- IOC reputation querying (VirusTotal, AbuseIPDB, OTX)
- Disk image timeline analysis with Plaso
- Volatility3 memory analysis guidance
- MITRE ATT&CK technique mapping
- Risk scoring logic and report templates
- Sentinel + XSOAR playbook templates
- Atomic Red Team validation framework

---

## 📁 Repository Structure
```
/forensic-toolkit-v2
├── KQL_Scripts/                      # Advanced hunting scripts
├── Python_Scripts/                  # IOC enrichment + phishing tools
├── IOC_Integration/                 # Threat intel pullers (VT, OTX, AbuseIPDB)
├── Memory_Acquisition/             # RAM capture scripts
├── Disk_Analysis/                  # Plaso timeline commands
├── Sentinel_Playbooks/            # JSON playbook templates for automation
├── XSOAR_Playbooks/               # YAML playbooks for Cortex
├── Simulation_Tests/              # Atomic Red Team test logic
├── Reporting/                      # PDF/DOCX report templates
└── README.md                       # This file
```

---

## 🚀 Quick Start
1. Clone the repository:
   ```bash
   git clone https://github.com/your-org/forensic-toolkit-v2.git
   ```
2. Open `KQL_Scripts/` and test queries in Defender/Sentinel
3. Run `.py` tools from `Python_Scripts/` or `IOC_Integration/`
4. Import JSON/YAML playbooks into your SOAR platform
5. Use `Reporting/incident_summary_template.docx` for executive writeups

---

## 🧠 Prerequisites
- Microsoft 365 Defender + Sentinel access
- Python 3.8+ with `requests`, `email`
- API keys for VirusTotal, AbuseIPDB, and OTX
- FTK Imager / Belkasoft RAM Capture (for memory acquisition)
- Plaso, Timesketch, or Autopsy for disk forensics

---

## 🎯 Use Cases
- Confirm persistence or reentry after phishing
- Detect lateral movement or logon anomalies
- Verify unauthorized software installations (e.g., DWAgent)
- Reconstruct attacker timelines
- Enrich IOCs before threat sharing or blocking

---

## 🧪 Validation Support
Run tests in `Simulation_Tests/` to simulate phishing, process injection, and C2 beaconing. Validate against included KQL.

---

## 🏁 Roadmap
- [x] IOC feed integration
- [x] Sentinel playbook support
- [ ] XDR integration (CrowdStrike, Cortex XDR)
- [ ] Jupyter-based correlation notebook
- [ ] Web dashboard with timeline overlays

---

## 🤝 Contributing
All detection engineers, DFIR analysts, and red teamers are welcome.
- Fork the repo
- Add features or playbooks
- Submit PRs with notes on MITRE TTP coverage

---

## 📜 License
MIT License
