# Lab 5 – Mobile Application Testing

## Objective
To analyze Android applications for static and dynamic security vulnerabilities.

## Tools Used
- MobSF
- Frida
- Drozer
- Android Emulator / Test APK

## Tasks Performed
1. Performed static analysis using MobSF.
2. Identified insecure storage vulnerabilities.
3. Hooked authentication logic using Frida.
4. Tested IPC exposure using Drozer.

## Key Findings
- Insecure storage detected (High severity).
- Authentication bypass achieved via runtime hooking.
- Exposed IPC components identified.

## Evidence
- MobSF reports in `Reports/`
- Frida hook screenshots in `Screenshots/`

## Outcome
Sensitive application logic successfully bypassed at runtime.

## Mitigation Recommendations
- Encrypt sensitive data at rest
- Implement runtime integrity checks
- Restrict exported IPC components
