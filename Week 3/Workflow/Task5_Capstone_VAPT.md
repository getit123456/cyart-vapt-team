# Task 5 – Capstone Project: Full VAPT Cycle

## Objective
To perform an end-to-end Vulnerability Assessment and Penetration Testing (VAPT)
cycle aligned with PTES methodology.

## Target Details
- Target System: Metasploitable2
- Target IP: 192.168.56.102

## Tools Used
- Nmap
- OpenVAS
- Metasploit Framework
- Wireshark
- Google Docs

## PTES Phases

### 1. Discovery & Enumeration
Nmap was used to identify open ports and services.

### 2. Vulnerability Detection
OpenVAS was used to perform an automated vulnerability scan.

| Timestamp | Target IP | Vulnerability | PTES Phase |
|---------|-----------|---------------|-----------|
| 2025-12-19 10:30 | 192.168.56.102 | vsftpd Backdoor RCE | Exploitation |

### 3. Exploitation
The vsftpd 2.3.4 vulnerability was exploited using Metasploit, resulting in root
shell access.

### 4. Post-Exploitation
System access was verified and evidence was collected following forensic best
practices.

### 5. Remediation
Recommendations included disabling insecure services, applying patches, and
restricting network access.

### 6. Verification
A follow-up scan was conceptually performed to validate remediation effectiveness.

## Conclusion
The capstone project demonstrated a complete VAPT lifecycle, from discovery to
reporting, reflecting real-world penetration testing workflows.

## Screenshots

![Nmap Scan](../Screenshots/Task1/nmap_full_scan.png)
![Metasploit Exploit](../Screenshots/Task1/metasploit_exploit.png)
![Post Exploitation](../Screenshots/Task4/root_access.png)
![Wireshark Evidence](../Screenshots/Task4/wireshark_capture.png)
