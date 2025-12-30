
---

# LAB 5 – Mobile Application Testing  
```md
# Lab 5 – Mobile Application Testing Workflow

## Objective
To identify mobile application vulnerabilities using static and dynamic analysis.

## Tools Used
- MobSF
- Frida
- Drozer
- Android Emulator

## Step-by-Step Workflow

### Step 1: Static Analysis (MobSF)
- Upload APK to MobSF
- Review permissions and insecure storage issues

### Step 2: Dynamic Analysis (Frida)
Create authentication bypass script.

frida -U -f com.android.insecurebankv2 -l bypass.js

### Step 3: IPC Testing (Drozer)

Identify exported activities and services.

### Step 4: Validation

Confirm authentication bypass without valid credentials.

## Evidence

MobSF vulnerability report

Frida console output

## Outcome

Authentication bypass and insecure storage identified.
