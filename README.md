# IOC-Alert-Analysis-and-Incident-Reporting

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
    └── IOC-Alert-05.pdf
```

## 📄 Incident Reports Summary

| Report | Alert Type | Severity | Key IOC Type(s) | Status |
|--------|-----------|----------|------------------|--------|
| IOC-Alert-01 | *e.g. Phishing Attempt* | *Medium* | *Domain, URL* | Resolved |
| IOC-Alert-02 | *e.g. Malware Detection* | *High* | *File Hash, IP* | Resolved |
| IOC-Alert-03 | *e.g. Suspicious Login* | *Low* | *IP Address* | Resolved |
| IOC-Alert-04 | *e.g. C2 Communication* | *High* | *Domain, IP* | Resolved |
| IOC-Alert-05 | *e.g. Data Exfiltration Attempt* | *Critical* | *IP, File Hash* | Resolved |

> Update this table with the real alert types, severities, and IOC categories from your reports.

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

*(Update with what you actually used)*
- SIEM log analysis
- VirusTotal / threat intelligence lookups
- Wireshark / network traffic analysis
- MITRE ATT&CK framework mapping

## 📚 Frameworks Referenced

- [NIST SP 800-61: Computer Security Incident Handling Guide](https://csrc.nist.gov/pubs/sp/800/61/r2/final)
- [SANS Incident Response Process (PICERL)](https://www.sans.org/)
- [MITRE ATT&CK Framework](https://attack.mitre.org/)

## ⚠️ Disclaimer

All incidents documented in this repository are simulated or based on publicly available training scenarios. No real organizational data, confidential information, or personally identifiable information (PII) is included.

## 👤 Author

**Harshitha BR**
Cybersecurity Enthusiast | Aspiring SOC Analyst
[LinkedIn](#) • [GitHub](#) • [Email](#)

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
