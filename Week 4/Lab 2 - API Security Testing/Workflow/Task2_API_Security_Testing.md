
---

#  LAB 2 – API Security Testing  
```md
# Lab 2 – API Security Testing Workflow

## Objective
To identify and exploit API vulnerabilities based on OWASP API Top 10.

## Tools Used
- Burp Suite
- Postman
- sqlmap
- DVWA API

## Step-by-Step Workflow

### Step 1: API Endpoint Discovery
Intercept API traffic using Burp Proxy.
- Enable proxy
- Browse application
- Identify `/api/*` endpoints

### Step 2: Broken Object Level Authorization (BOLA)
Modify object IDs in requests.
```http
GET /api/users/2

Change ID to another user and observe unauthorized access.

### Step 3: Token Manipulation

Remove Authorization header

Replay request via Burp Repeater

Validate access control failure

### Step 4: GraphQL Injection

Use Postman to send malicious GraphQL queries.

{
  "query": "{ users { id password } }"
}

### Step 5: Validation

Confirm data leakage or unauthorized access.

## Evidence

Burp request/response screenshots

API payload logs

## Outcome

Critical BOLA and GraphQL injection vulnerabilities identified.
