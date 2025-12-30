# Lab 6 – Capstone VAPT Engagement

## Objective
To conduct a full PTES-based Vulnerability Assessment and Penetration Testing (VAPT) engagement.

## Tools Used
- Kali Linux
- Metasploit
- OpenVAS
- Burp Suite

## Engagement Scope
- Target: HackTheBox / VulnHub VM
- Methodology: PTES

## Activities Performed
1. Planning and reconnaissance
2. Vulnerability scanning with OpenVAS
3. Exploitation using Metasploit (VSFTPD backdoor)
4. API testing using Burp Suite
5. Post-exploitation and cleanup

## Key Findings
- Remote Code Execution via VSFTPD
- Multiple misconfigurations identified

## Evidence
- Scan reports in `Reports/`
- Exploitation screenshots in `Screenshots/`

## Remediation Summary
- Patch vulnerable services
- Enforce least privilege
- Implement network segmentation

## Outcome
Successful end-to-end penetration test with remediation validation.
