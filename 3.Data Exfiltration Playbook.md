# Data Exfiltration Playbook

### 1. Detection & Analysis
- [ ] **Identify Volume:** Determine the amount of data transferred (MB/GB) using Netflow or Firewall logs.
- [ ] **Identify Data:** Check DLP (Data Loss Prevention) logs to see which files or keywords triggered the alert.
- [ ] **Destination:** Research the destination IP/Domain (e.g., a known file-sharing site like Mega.nz).

### 2. Containment
- [ ] **Kill Connections:** Immediately terminate any active network sessions between the host and the destination.
- [ ] **Disable Account:** Disable the account used to access the data.

### 3. Eradication & Recovery
- [ ] **Takedown:** Contact the hosting provider of the destination IP to request a takedown of the uploaded data.
- [ ] **Vulnerability Fix:** Block the protocol used for exfiltration (e.g., FTP, SSH) if not business-required.

### 4. Post-Incident
- [ ] **Legal/Compliance:** Notify the Legal or Privacy team if PII (Personally Identifiable Information) was leaked.
