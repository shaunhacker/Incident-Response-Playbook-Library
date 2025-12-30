# Brute Force Attack Playbook

### 1. Detection & Analysis
- [ ] **Verify Source:** Check if the source IP is a known VPN, Tor exit node, or proxy.
- [ ] **Success Check:** Filter SIEM logs for "4624" (Success) immediately following "4625" (Failure) from the same IP.
- [ ] **Account Scope:** Determine if the attack is targeting one account (brute force) or many (password spraying).

### 2. Containment
- [ ] **IP Blocking:** Block the attacking IP at the Edge Firewall or WAF.
- [ ] **Account Lockout:** Temporarily disable targeted accounts if they do not have an automated lockout policy.

### 3. Eradication & Recovery
- [ ] **Password Reset:** Force a password reset for any accounts that show a "Successful Login" from the attacker's IP.
- [ ] **Enable MFA:** Ensure MFA is enforced for all external-facing login portals.

### 4. Post-Incident
- [ ] **Policy Review:** Adjust account lockout thresholds to be more restrictive if necessary.
