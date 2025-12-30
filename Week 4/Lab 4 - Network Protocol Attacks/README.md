# Lab 4 – Network Protocol Attacks

## Objective
To perform Man-in-the-Middle (MitM) attacks and exploit insecure network protocols.

## Tools Used
- Responder
- Ettercap
- Wireshark
- TryHackMe VM

## Tasks Performed
1. Captured NTLM hashes using Responder.
2. Executed SMB relay attack.
3. Performed ARP spoofing using Ettercap.
4. Analyzed intercepted traffic with Wireshark.

## Key Findings
- NTLM hashes successfully captured.
- Sensitive credentials exposed via MitM.
- Encrypted traffic metadata analyzed.

## Evidence
- Packet captures stored in `Screenshots/`
- Attack logs documented in `Reports/`

## Outcome
Credential interception and traffic manipulation were successfully demonstrated.

## Mitigation Recommendations
- Disable LLMNR/NBT-NS
- Enforce SMB signing
- Use encrypted protocols
