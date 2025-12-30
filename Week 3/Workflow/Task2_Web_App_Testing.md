# Task 2 – Web Application Penetration Testing

## Objective
To identify and exploit common web application vulnerabilities using manual and
automated testing techniques.

## Target Application
- Application: Damn Vulnerable Web Application (DVWA)
- Platform: Metasploitable2

## Tools Used
- DVWA
- Burp Suite
- sqlmap
- Web Browser

## Steps Performed

### Step 1: DVWA Setup
The DVWA application was accessed and the security level was set to Low to allow
testing of vulnerabilities.

### Step 2: SQL Injection Testing
Manual SQL Injection was performed on the SQL Injection module.

Payload used:
' OR '1'='1 --

The application returned multiple database records, confirming SQL Injection.

### Step 3: Cross-Site Scripting (XSS)
Reflected XSS was tested using the following payload:

<script>alert(1)</script>

The payload executed successfully, confirming the vulnerability.

### Step 4: Burp Suite Interception
Burp Suite was configured as a proxy to intercept HTTP requests. Session cookies
were observed in plaintext, indicating insecure session handling.

## Findings Summary

| Test ID | Vulnerability | Severity |
|-------|---------------|----------|
| 001 | SQL Injection | Critical |
| 002 | Reflected XSS | Medium |

## Conclusion
The application suffers from multiple OWASP Top 10 vulnerabilities caused by
improper input validation and insecure session management.

## Screenshots

![DVWA Dashboard](../Screenshots/Task2/dvwa_dashboard.png)
![Security Level Low](../Screenshots/Task2/security_low.png)
![SQL Injection Success](../Screenshots/Task2/sql_injection_success.png)
![XSS Injection](../Screenshots/Task2/xss_injection.png)
![Reflected XSS](../Screenshots/Task2/xss_reflected.png)

