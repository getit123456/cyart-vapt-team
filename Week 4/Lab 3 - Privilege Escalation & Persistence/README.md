# Lab 3 – Privilege Escalation and Persistence

## Objective
To escalate privileges on a compromised system and establish persistence mechanisms.

## Tools Used
- Meterpreter
- LinPEAS
- PowerSploit
- VulnHub VM

## Tasks Performed
1. Ran LinPEAS to enumerate privilege escalation vectors.
2. Identified misconfigured SUID binaries.
3. Exploited SUID vulnerability to obtain root shell.
4. Established persistence using cron job execution.

## Key Findings
- Multiple privilege escalation vectors identified.
- Successful escalation to root user.
- Persistence maintained after system reboot.

## Evidence
- Enumeration outputs in `Reports/`
- Privilege escalation screenshots in `Screenshots/`

## Outcome
Full system compromise with persistent access achieved.

## Mitigation Recommendations
- Remove unnecessary SUID permissions
- Monitor cron jobs and startup scripts
- Apply least privilege principle
