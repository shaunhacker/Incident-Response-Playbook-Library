# Incident Response Playbook Library

## 📌 Overview
This repository contains a collection of standardized **Incident Response (IR) Playbooks** designed to guide SOC Analysts through the identification, containment, and recovery of common security threats. 

Each playbook follows the **NIST SP 800-61** framework (Preparation, Detection & Analysis, Containment, Eradication & Recovery, and Post-Incident Activity).

## 🛠️ Purpose
The goal of this project is to demonstrate a process-oriented mindset and technical readiness for a SOC Analyst role. These playbooks ensure that response actions are:
* **Consistent:** Reducing human error during high-pressure incidents.
* **Efficient:** Minimizing "Mean Time to Respond" (MTTR).
* **Measurable:** Providing a checklist for post-incident reporting.

---

## 📖 Playbook Directory

| Incident Type | Description | Link |
| :--- | :--- | :--- |
| **Phishing** | Investigation of suspicious emails, URL analysis, and credential harvesting. | [View Playbook](phishing-response.md) |
| **Malware Infection** | Handling endpoint infections, persistence mechanisms, and C2 communication. | [View Playbook](malware-response.md) |
| **Brute Force** | Responding to automated login attempts and password spraying. | [View Playbook](brute-force-response.md) |
| **Account Compromise** | Managing unauthorized access, session revocation, and lateral movement. | [View Playbook](unauthorized-access.md) |
| **Data Exfiltration** | Detecting and stopping unauthorized data transfers to external sources. | [View Playbook](data-exfiltration.md) |

---

## 🚀 Methodology
These playbooks are structured to be used alongside a **SIEM** (e.g., Splunk, Sentinel) and **EDR** (e.g., CrowdStrike, Microsoft Defender). 

### Key Steps Followed:
1. **Detection & Analysis:** Alert validation and scoping.
2. **Containment:** Stopping the "bleeding" (isolating hosts, disabling accounts).
3. **Eradication:** Removing the root cause (deleting malware, patching).
4. **Recovery:** Restoring systems to normal operations.
5. **Lessons Learned:** Analyzing the incident to prevent future occurrences.

---

## 📈 Future Improvements
- [ ] Integration with Sigma/YARA rules for automated detection.
- [ ] Conversion of Markdown playbooks into automated SOAR workflows (Python/Tines).
- [ ] Mapping each playbook directly to **MITRE ATT&CK** techniques.

---
**Contact:** [Your Name] - [Link to LinkedIn]
