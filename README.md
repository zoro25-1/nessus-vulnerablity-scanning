# nessus-vulnerablity-scanning
#  Task 3: Basic Vulnerability Scan on Windows

##  Objective
Perform a basic vulnerability scan on a Windows PC using Nessus Essentials to identify common security risks and understand how vulnerability scanners work.

---

##  Tools Used
- **Nessus Essentials** (Free version)
- **Target:** Localhost (`127.0.0.1`) / Local IP (`192.168.56.1`)
- **Scan Type:** Full system scan



##  Summary of Findings
The scan revealed several informational and low-risk vulnerabilities. Below are the most notable:

### 1. **Windows NetBIOS / SMB Remote Host Information Disclosure**
- **Port:** 445
- **Risk:** Information Disclosure
- **Synopsis:** Host responds to NetBIOS/SMB requests, revealing computer and domain name.
- **Fix:** Disable NetBIOS over TCP/IP if not needed.

### 2. **DCE Services Enumeration**
- **Port:** 135
- **Risk:** Information Disclosure
- **Synopsis:** RPC services are exposed and can be enumerated.
- **Fix:** Restrict access to port 135 using firewall rules.

### 3. **Nessus Server Detection**
- **Port:** 8834
- **Risk:** Informational
- **Synopsis:** Nessus daemon is detected on the scan port.
- **Fix:** Ensure Nessus is properly secured and authorized.



##  Screenshots
Screenshots of the scan results are included in the `/screenshots` folder.



##  Key Concepts
- Vulnerability Scanning vs. Penetration Testing
- CVSS Scoring
- Risk Prioritization
- Remediation Techniques

