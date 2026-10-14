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
| **Phishing** | Investigation of suspicious emails, URL analysis, and credential harvesting. | [View Playbook](1.Phishing%20Incident%20Response%20Playbook.md) |
| **Brute Force** | Responding to automated login attempts and password spraying. | [View Playbook](2.Brute%20Force%20Attack%20Playbook.md) |
| **Data Exfiltration** | Detecting and stopping unauthorized data transfers to external sources. | [View Playbook](3.Data%20Exfiltration%20Playbook.md) |
| **Malware Infection** | Handling endpoint infections, persistence mechanisms, and C2 communication. | [View Playbook](4.Malware%20Infection%20Playbook.md) |
| **Account Compromise** | Managing unauthorized access, session revocation, and lateral movement. | [View Playbook](5.Unauthorized%20Access%20Playbook.md) |
| **Incident Case Report** | Standardized reporting template for documenting completed incidents. | [View Playbook](6.Incident%20Case%20Report.md) |

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
**Contact:** Thando Hlakanyana - www.linkedin.com/in/thando-hlakanyana
