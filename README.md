# IOC Alert Analysis and Incident Reporting

A collection of simulated security incident investigations, documenting the identification, analysis, and reporting of Indicators of Compromise (IOCs) across multiple alert scenarios. This repository demonstrates a structured, analyst-driven approach to incident detection, triage, and response reporting.

## 📌 Overview

Each report in this repository represents an end-to-end walkthrough of a security alert — from initial detection through IOC extraction, threat classification, and final incident documentation. The goal is to showcase practical SOC/incident response workflows using industry-standard analysis methodology.

## 🎯 Objectives

- Practice identifying and documenting Indicators of Compromise (IPs, hashes, domains, URLs, file artifacts)
- Apply structured incident reporting aligned with industry frameworks (NIST 800-61 / SANS PICERL)
- Map findings to the MITRE ATT&CK framework where applicable
- Build a repeatable, professional reporting template usable in real SOC environments

## 🗂️ Repository Structure

```
IOC-Alert-Analysis-and-Incident-Reporting/
├── README.md
├── LICENSE
└── Incident-Reports/
    ├── IOC-Alert-01.pdf
    ├── IOC-Alert-02.pdf
    ├── IOC-Alert-03.pdf
    ├── IOC-Alert-04.pdf
    
```

## 📄 Incident Reports Summary

| Report | Alert Type | Source | Severity | Key IOC(s) | Validity |
|--------|-----------|--------|----------|------------|----------|
| [IOC-Alert-01](Incident-Reports/IOC-Alert-01.pdf) | Client-Side SSH Exploitation Attempt (CVE-2026-55200, libssh2) | Splunk | Critical | Malicious SSH server `172.67.212.45`, source `185.220.101.45` | ✅ True Positive |
| [IOC-Alert-02](Incident-Reports/IOC-Alert-02.pdf) | Suspicious PowerShell Privilege Escalation | Microsoft Defender for Endpoint | Critical | Tor exit node IP `185.220.101.5` | ✅ True Positive |
| [IOC-Alert-03](Incident-Reports/IOC-Alert-03.pdf) | Suspicious AzureMetrics Activity | Microsoft Sentinel | High | IP `88.235.4.157` (Turkey, no vendor detections) | ❌ False Positive |
| [IOC-Alert-04](Incident-Reports/IOC-Alert-04.pdf) | Log4Shell Remote Code Execution (CVE-2021-44228) | Microsoft Sentinel | Low | `${jndi:...}` JNDI payload, IP `192.52.194.205` | ✅ True Positive |

## 🎯 MITRE ATT&CK Mapping

| Report | Technique | Tactic |
|--------|-----------|--------|
| IOC-Alert-01 | T1203 – Exploitation for Client Execution | Execution |
| IOC-Alert-02 | T1059.001 – PowerShell / T1068 – Exploitation for Privilege Escalation | Execution, Privilege Escalation |
| IOC-Alert-04 | T1190 – Exploit Public-Facing Application | Initial Access |

## 🧩 Report Methodology

Each incident report follows a consistent analytical structure:

1. **Alert Summary** — trigger source and initial detection details
2. **Timeline of Events** — chronological sequence from detection to resolution
3. **Indicators of Compromise (IOCs)** — extracted artifacts (IPs, hashes, domains, etc.)
4. **Analysis** — correlation, threat intelligence lookups, and classification
5. **MITRE ATT&CK Mapping** — relevant tactics and techniques identified
6. **Response Actions** — containment, eradication, and recovery steps
7. **Recommendations** — preventive measures and lessons learned

## 🛠️ Tools & Techniques Referenced

- **SIEM platforms:** Splunk Cloud, Microsoft Sentinel
- **EDR:** Microsoft Defender for Endpoint
- **Threat Intelligence:** VirusTotal (IOC reputation lookups)
- **IP/Geolocation Enrichment:** IP2Location, WhatIsMyIPAddress
- **MITRE ATT&CK framework mapping**
- **CVE correlation:** NVD / vendor advisories (CVE-2026-55200, CVE-2021-44228)

## 📚 Frameworks Referenced

- [NIST SP 800-61: Computer Security Incident Handling Guide](https://csrc.nist.gov/pubs/sp/800/61/r2/final)
- [SANS Incident Response Process (PICERL)](https://www.sans.org/)
- [MITRE ATT&CK Framework](https://attack.mitre.org/)

## ⚠️ Disclaimer

All incidents documented in this repository are simulated or based on publicly available training scenarios. No real organizational data, confidential information, or personally identifiable information (PII) is included.

## 👤 Author

**Harshitha BR**
Cybersecurity Enthusiast | Aspiring SOC Analyst
https://www.linkedin.com/in/b-r-harshitha-17769b383/(#) • https://github.com/harshithabrreddy(#) •harshithabrreddy@gmail.com(#)

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
