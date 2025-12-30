# Incident Case Report: [Case #ID-12345]

## 1. Executive Summary
**Incident Title:** [e.g., Targeted Phishing & Account Compromise]
**Severity:** 🔴 High / 🟡 Medium / 🔵 Low
**Status:** [Resolved / Under Investigation]
**Date Identified:** YYYY-MM-DD
**Primary Analyst:** [Your Name]

**Summary:** Provide a 2-3 sentence overview. (e.g., An employee in Finance was targeted by a phishing email which led to a successful credential harvest and unauthorized login from a foreign IP.)

---

## 2. Incident Timeline
| Time (UTC) | Action/Event | Description |
| :--- | :--- | :--- |
| 09:00 | **Alert** | SIEM triggered 'Impossible Travel' alert for user J. Doe. |
| 09:15 | **Triage** | Analyst verified login was from a known Tor Exit Node. |
| 09:30 | **Containment** | User account disabled; all active sessions revoked. |
| 10:00 | **Eradication** | Malicious Outlook forwarding rules removed. |

---

## 3. Technical Analysis
* **Indicators of Compromise (IOCs):**
    * **IP Address:** `192.x.x.x` (Attacker Source)
    * **Malicious URL:** `hxxp://legit-service-login[.]com`
    * **User Agent:** `Mozilla/5.0 (Windows NT 10.0; Win64; x64)...`
* **Attack Vector:** Explain how they got in (e.g., Phishing link leading to a fake Microsoft 365 login page).
* **Tools Used:** (e.g., Splunk for log analysis, VirusTotal for URL reputation, Azure AD for session revocation).

---

## 4. Playbook Alignment
This incident was handled following the **[Unauthorized Access Playbook](./unauthorized-access.md)**. 
- [x] Detection & Analysis
- [x] Containment
- [x] Eradication & Recovery
- [x] Post-Incident Activity

---

## 5. Root Cause & Lessons Learned
* **Root Cause:** User lacked MFA (Multi-Factor Authentication) on their secondary administrative account.
* **Recommendations:** 1. Enforce MFA across **all** accounts without exception.
    2. Implement geo-blocking at the firewall for non-business-operating regions.
    3. Conduct a phishing simulation for the Finance department.

---

## 6. Evidence & Artifacts
> *Insert screenshots of SIEM alerts, firewall logs, or email headers here to prove the investigation.*
