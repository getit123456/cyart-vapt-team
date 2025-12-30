# Lab 2 – API Security Testing

## Objective
To identify and exploit API vulnerabilities aligned with the OWASP API Top 10 using both automated and manual testing techniques.

## Tools Used
- Burp Suite
- Postman
- sqlmap
- DVWA API

## Tasks Performed
1. Enumerated API endpoints using Burp Suite.
2. Tested for Broken Object Level Authorization (BOLA).
3. Manipulated API tokens to gain unauthorized access.
4. Fuzzed GraphQL queries using Postman.
5. Validated SQL injection risks using sqlmap.

## Vulnerabilities Identified
- Broken Object Level Authorization (Critical)
- GraphQL Injection (High)

## Evidence
- Request/response captures stored in `Screenshots/`
- API test results summarized in `Reports/`

## Outcome
Unauthorized access to sensitive API resources was achieved.

## Mitigation Recommendations
- Implement strict object-level authorization
- Validate tokens server-side
- Apply GraphQL query depth and complexity limits
