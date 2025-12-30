# Unauthorized Access Playbook

### 1. Detection & Analysis
- [ ] **Log Correlation:** Review sign-in logs for "Impossible Travel" or "Unfamiliar Properties" alerts.
- [ ] **Identify Actions:** Use Audit Logs to see what the attacker did (e.g., data accessed, mail forwarding rules created).

### 2. Containment
- [ ] **Revoke Sessions:** Terminate all active O365/Azure/AWS sessions for the compromised user.
- [ ] **Reset Credentials:** Change the password and verify that the "Recovery Email/Phone" hasn't been changed.

### 3. Eradication & Recovery
- [ ] **Remove Backdoors:** Delete any malicious mail rules, new SSH keys, or newly created admin accounts.
- [ ] **System Review:** Check for lateral movement from the compromised account to other sensitive systems.

### 4. Post-Incident
- [ ] **Root Cause:** Determine how the account was taken (Phishing? Credential Leak?) and address the gap.
