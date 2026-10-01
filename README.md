# enterprise-soc-lab

SOC Detection Lab

A hands-on Security Operations Center (SOC) lab focused on security monitoring, threat detection, alert triage, log analysis, incident investigation, and Blue Team operations.

🎯 Project Objectives

This project simulates a small SOC environment where security events are generated, collected, detected, investigated, and documented.

The main objectives are to:

- Build practical SOC L1 investigation skills
- Understand security telemetry and log sources
- Develop and test detection rules
- Investigate suspicious activity and security alerts
- Practice evidence collection and analysis
- Map observed activity to the MITRE ATT&CK framework
- Document incidents using a structured investigation process

🏗️ Lab Architecture

The lab will contain multiple systems representing a simplified enterprise environment:

                    ┌─────────────────┐
                    │    Attacker     │
                    │   Simulation    │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │   Windows Host  │
                    │   / Endpoints   │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Network / IDS   │
                    │   Telemetry     │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │      SIEM       │
                    │     Splunk      │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ SOC Analyst     │
                    │ Detection &     │
                    │ Investigation   │
                    └─────────────────┘

The architecture will evolve as additional telemetry sources and detection capabilities are added.

🔎 SOC Workflow

The investigations in this project follow a structured workflow:

Alert
  ↓
Validate
  ↓
Triage
  ↓
Collect Evidence
  ↓
Investigate
  ↓
Determine Severity
  ↓
Document Findings
  ↓
Escalate / Close

The goal is to practice the reasoning process used during real SOC investigations rather than simply identifying individual commands or indicators.

🛡️ Detection & Investigation

The project will include detections and investigations involving areas such as:

- Windows authentication activity
- Suspicious process execution
- PowerShell activity
- Remote access activity
- Network scanning
- Brute-force behavior
- Suspicious network connections
- IDS/IPS alerts
- Endpoint telemetry
- Indicator of Compromise (IOC) analysis

Detection logic will be tested against generated security telemetry whenever possible.

🧰 Technologies

Planned technologies include:

- Splunk
- Windows Event Logs
- Sysmon
- Suricata
- Linux
- Windows
- PowerShell
- SPL
- Sigma
- MITRE ATT&CK
- Atomic Red Team

Additional tools may be added as the lab evolves.

📂 Repository Structure

SOC-Detection-Lab/
│
├── README.md
│
├── docs/
│   └── Lab documentation
│
├── detections/
│   └── Detection rules and queries
│
├── investigations/
│   └── Incident investigations
│
├── lab/
│   └── Lab configuration and setup
│
├── evidence/
│   └── Investigation evidence and exported telemetry
│
└── screenshots/
    └── Screenshots demonstrating the lab and investigations

📊 Investigation Documentation

Each investigation will document:

- Alert / detection
- Initial hypothesis
- Relevant logs
- Indicators of Compromise
- Timeline
- Analysis
- MITRE ATT&CK mapping
- Severity assessment
- Findings
- Recommended response
- Final disposition

⚠️ Disclaimer

This project is intended for educational and defensive security research purposes.

All attack simulations are performed in an isolated lab environment under controlled conditions.

🚧 Project Status

Status: In Development

The lab is being built incrementally, with new telemetry sources, detections, and investigations added over time.
