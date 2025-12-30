# Week 2 – VAPT Workflow (CyArt Team)

## 1. Environment Setup
- Attacker: Kali Linux
- Target: Metasploitable2
- Network: Host-only Adapter

## 2. Reconnaissance
- Nmap full port scan
- Service enumeration
- Apache directory listing discovered

(Screenshot: nmap_scan.png)

## 3. Vulnerability Assessment
### 3.1 SQL Injection (DVWA)
- Tool: sqlmap
- Target: /dvwa/vulnerabilities/sqli
- Result: SQL Injection confirmed (MySQL)

(Screenshots: sqlmap_injection.png, db_dump.png)

### 3.2 Command Execution
- Tool: DVWA
- Payload: ; whoami
- Result: Command execution achieved

(Screenshot: command_execution.png)

### 3.3 File & Directory Exposure
- Exposed paths: /doc, /icons
- phpinfo.php exposed revealing PHP version

(Screenshots: index_doc.png, phpinfo.png)

## 4. Exploitation
- Metasploit used against vsftpd backdoor
- Meterpreter shell obtained
- Privilege escalation confirmed (root)

(Screenshots: meterpreter.png)

## 5. Evidence Collection
- Extracted config files
- Hashing using sha256sum
- SQLmap output stored

(Screenshots: hashes.png)

## 6. Conclusion
The target system was critically vulnerable due to outdated services, misconfigurations, and lack of input validation. Full compromise was achieved.
