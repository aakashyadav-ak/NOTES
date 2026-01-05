
# OWASP MOBILE TOP 10 (2024)
## M01:2024 - Improper Credential Usage
- [ ] Hardcoded API Keys in Source Code
- [ ] Hardcoded Passwords in Code
- [ ] Hardcoded Secrets in strings.xml/plist
- [ ] Credentials in BuildConfig Files
- [ ] API Keys in AndroidManifest.xml/Info.plist
- [ ] Secrets in Native Libraries (.so files)
- [ ] Credentials Logged in Logcat/Console
- [ ] Credentials in Crash Reports
- [ ] Shared Credentials Across Users
- [ ] Credentials in Memory (Runtime Analysis)
- [ ] Credentials in Clipboard
- [ ] OAuth Token Mishandling
- [ ] Firebase/AWS Keys Exposure
- [ ] Third-party SDK Credentials Exposure

## M02:2024 - Inadequate Supply Chain Security
- [ ] Outdated Libraries with Known CVEs
- [ ] Vulnerable Third-party SDKs
- [ ] Malicious Dependencies
- [ ] Unverified Library Sources
- [ ] Missing Integrity Verification
- [ ] Dependency Confusion Attacks
- [ ] Compromised SDK Updates
- [ ] Unsigned Libraries
- [ ] Typosquatting Libraries
- [ ] Abandoned/Unmaintained Libraries
- [ ] License Compliance Issues
- [ ] Transitive Dependency Vulnerabilities
- [ ] Debug SDKs in Production

## M03:2024 - Insecure Authentication/Authorization
### Authentication Flaws
- [ ] Weak Password Policy Acceptance
- [ ] No Account Lockout Mechanism
- [ ] Brute Force Attack Success
- [ ] Credential Stuffing Vulnerability
- [ ] Biometric Authentication Bypass
- [ ] Local Authentication Bypass
- [ ] Remember Me Token Weakness
- [ ] Insecure "Forgot Password" Flow
- [ ] SMS OTP Interception
- [ ] 2FA/MFA Bypass Techniques
- [ ] Session Token Predictability
- [ ] Session Not Invalidated on Logout
- [ ] Session Not Invalidated on Password Change
- [ ] Concurrent Session Issues
- [ ] Device Binding Bypass

### Authorization Flaws
- [ ] IDOR (Insecure Direct Object Reference)
- [ ] Horizontal Privilege Escalation
- [ ] Vertical Privilege Escalation
- [ ] Missing Function Level Access Control
- [ ] Role Manipulation
- [ ] API Authorization Bypass
- [ ] Client-Side Authorization Checks
- [ ] JWT Token Manipulation
- [ ] OAuth Scope Bypass
- [ ] Deep Link Authorization Bypass

## M04:2024 - Insufficient Input/Output Validation
### Injection Attacks
- [ ] SQL Injection in Local DB
- [ ] SQL Injection via API
- [ ] NoSQL Injection
- [ ] LDAP Injection
- [ ] XML Injection
- [ ] XPath Injection
- [ ] OS Command Injection
- [ ] Format String Vulnerabilities

### Client-Side Injection
- [ ] XSS in WebView (Reflected)
- [ ] XSS in WebView (Stored)
- [ ] XSS in WebView (DOM-based)
- [ ] JavaScript Interface Exploitation
- [ ] HTML Injection
- [ ] CSS Injection

### File-Based Attacks
- [ ] Path Traversal (Local Files)
- [ ] Local File Inclusion
- [ ] Zip Slip Vulnerability
- [ ] File Upload Vulnerabilities
- [ ] Content Provider Path Traversal

### Other Validation Issues
- [ ] Buffer Overflow
- [ ] Integer Overflow
- [ ] Input Length Bypass
- [ ] Special Character Bypass
- [ ] Unicode/Encoding Bypass
- [ ] Null Byte Injection

## M05:2024 - Insecure Communication
### TLS/SSL Issues
- [ ] HTTP Traffic (Cleartext)
- [ ] Mixed Content (HTTP + HTTPS)
- [ ] Weak TLS Versions (TLS 1.0/1.1)
- [ ] Weak Cipher Suites
- [ ] Invalid Certificate Acceptance
- [ ] Self-Signed Certificate Acceptance
- [ ] Hostname Verification Bypass
- [ ] Certificate Expiry Not Checked

### Certificate Pinning
- [ ] No Certificate Pinning
- [ ] Weak Pinning Implementation
- [ ] Certificate Pinning Bypass (Frida)
- [ ] Certificate Pinning Bypass (Objection)
- [ ] Backup Pin Exploitation

### Data in Transit
- [ ] Sensitive Data in URL Parameters
- [ ] Sensitive Data in HTTP Headers
- [ ] Credentials Sent Over HTTP
- [ ] Session Tokens Over HTTP
- [ ] PII Transmitted Unencrypted
- [ ] API Keys in Transit (Unprotected)

### Network Attacks
- [ ] Man-in-the-Middle (MITM) Success
- [ ] SSL Stripping Attack
- [ ] ARP Spoofing Vulnerability
- [ ] DNS Spoofing Vulnerability
- [ ] WebSocket Security Issues

## M06:2024 - Inadequate Privacy Controls
### Data Collection Issues
- [ ] Excessive Permissions Requested
- [ ] Unnecessary Data Collection
- [ ] Location Tracking Without Consent
- [ ] Contact Access Without Justification
- [ ] Camera/Microphone Abuse
- [ ] Device Identifiers Collection (IMEI/UDID)
- [ ] Advertising ID Misuse

### Data Exposure
- [ ] PII in Application Logs
- [ ] PII in Crash Reports
- [ ] PII Sent to Third-party Analytics
- [ ] User Data Shared Without Consent
- [ ] Clipboard Data Exposure
- [ ] Screenshot/Screen Recording Allowed
- [ ] Keyboard Cache Sensitive Data
- [ ] Pasteboard Persistence (iOS)

### Privacy Compliance
- [ ] Missing Privacy Policy
- [ ] Policy vs Behavior Mismatch
- [ ] No Data Deletion Option
- [ ] No Data Export Option
- [ ] Data Retention Issues
- [ ] Cross-border Data Transfer Issues
- [ ] Child Data Protection (COPPA)
- [ ] GDPR Compliance Issues

## M07:2024 - Insufficient Binary Protections
### Reverse Engineering
- [ ] No Code Obfuscation
- [ ] Readable Class/Method Names
- [ ] Decompilation Success (JADX/Hopper)
- [ ] String Encryption Missing
- [ ] Resource Encryption Missing
- [ ] Native Code Not Protected
- [ ] Debug Symbols Present

### Runtime Protection
- [ ] No Root/Jailbreak Detection
- [ ] Root Detection Bypass (Frida)
- [ ] Root Detection Bypass (Magisk Hide)
- [ ] No Emulator Detection
- [ ] Emulator Detection Bypass
- [ ] No Debugger Detection
- [ ] Debugger Attach Success
- [ ] No Frida/Xposed Detection
- [ ] Hooking Framework Success
- [ ] Memory Dump Success

### Integrity Protection
- [ ] No Tamper Detection
- [ ] APK Modification Success
- [ ] Repackaging Success
- [ ] Signature Verification Bypass
- [ ] Checksum Verification Missing
- [ ] Dynamic Loading Exploitation

## M08:2024 - Security Misconfiguration
### Android Specific
- [ ] android:debuggable="true"
- [ ] android:allowBackup="true"
- [ ] android:usesCleartextTraffic="true"
- [ ] Exported Activities (Unprotected)
- [ ] Exported Services (Unprotected)
- [ ] Exported Broadcast Receivers
- [ ] Exported Content Providers
- [ ] Intent Filter Vulnerabilities
- [ ] Pending Intent Vulnerabilities
- [ ] Task Hijacking Vulnerability
- [ ] Fragment Injection
- [ ] WebView JavaScript Enabled (Unsafe)
- [ ] WebView File Access Enabled
- [ ] WebView Universal Access Enabled
- [ ] Insecure Network Security Config

### iOS Specific
- [ ] ATS Disabled Entirely
- [ ] ATS Exceptions Too Broad
- [ ] Insecure URL Schemes
- [ ] Keychain Accessibility Issues
- [ ] Background Fetch Exposure
- [ ] Extension Data Sharing Issues
- [ ] Pasteboard Sharing Enabled
- [ ] Third-party Keyboard Allowed

### General Misconfigurations
- [ ] Debug Mode in Production
- [ ] Verbose Error Messages
- [ ] Default Credentials
- [ ] Test Accounts in Production
- [ ] Development Endpoints Exposed
- [ ] Unnecessary Features Enabled
- [ ] Insecure Deep Link Handling
- [ ] Custom URL Scheme Hijacking

## M09:2024 - Insecure Data Storage
### Shared Preferences / NSUserDefaults
- [ ] Passwords in SharedPreferences
- [ ] Tokens in SharedPreferences
- [ ] PII in SharedPreferences
- [ ] Sensitive Data in NSUserDefaults
- [ ] MODE_WORLD_READABLE Files
- [ ] MODE_WORLD_WRITEABLE Files

### Database Storage
- [ ] Unencrypted SQLite Database
- [ ] Sensitive Data in SQLite
- [ ] Realm Database Unencrypted
- [ ] Couchbase Lite Unencrypted
- [ ] Firebase Local Cache Exposure

### File Storage
- [ ] Sensitive Data in External Storage
- [ ] Sensitive Data in Cache Files
- [ ] Sensitive Data in Temp Files
- [ ] Log Files Contain Sensitive Data
- [ ] Backup Files Exposure
- [ ] WebView Cache Sensitive Data
- [ ] Cookie Storage Issues
- [ ] Screenshot Caching (Recent Apps)

### Secure Storage Issues
- [ ] Keystore/Keychain Not Used
- [ ] Weak Keystore Protection
- [ ] Extractable Keychain Items
- [ ] Hardware Security Module Not Used
- [ ] Biometric-Protected Keys Bypass

### Memory Issues
- [ ] Sensitive Data in Memory Dumps
- [ ] Credentials in Process Memory
- [ ] Memory Not Cleared After Use
- [ ] Swap File Data Exposure

## M10:2024 - Insufficient Cryptography
### Weak Algorithms
- [ ] MD5 Hashing Used
- [ ] SHA1 Hashing Used
- [ ] DES Encryption Used
- [ ] 3DES Encryption Used
- [ ] RC4 Encryption Used
- [ ] ECB Mode Used
- [ ] Weak Key Sizes (<2048 RSA, <256 AES)
- [ ] Broken Random Number Generator

### Key Management
- [ ] Hardcoded Encryption Keys
- [ ] Keys in Source Code
- [ ] Keys in Shared Preferences
- [ ] Keys in Strings Resources
- [ ] Predictable Key Generation
- [ ] Same Key for Multiple Purposes
- [ ] No Key Rotation
- [ ] Keys Transmitted in Cleartext

### Implementation Issues
- [ ] Custom Cryptography Implementation
- [ ] Improper IV/Nonce Usage
- [ ] IV/Nonce Reuse
- [ ] Missing Authentication (MAC)
- [ ] Padding Oracle Vulnerability
- [ ] Timing Side-Channel Attack
- [ ] Encryption Without Integrity

### Certificate Issues
- [ ] Self-Signed Certificates Accepted
- [ ] Certificate Validation Disabled
- [ ] Expired Certificates Accepted
- [ ] Wrong Host Certificates Accepted

---
```
┌─────────────────────────────────────────────────────────────┐
│  M1: IMPROPER CREDENTIAL USAGE                              │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ❌ WHAT'S WRONG:                                           │
│     App handles passwords/keys/tokens incorrectly           │
│                                                             │
│  📍 EXAMPLES:                                               │
│     • Hardcoded API keys in app code                        │
│     • Storing passwords in plain text                       │
│     • Using same credentials for all users                  │
│     • Credentials visible in app logs                       │
│                                                             │
│  🔍 HOW TO TEST:                                            │
│     1. Decompile app with JADX/APKTool                      │
│     2. Search for: "password", "api_key", "secret"          │
│     3. Check AndroidManifest.xml for exposed data           │
│     4. Review log files for credentials                     │
│                                                             │
│  ✅ PROPER FIX:                                             │
│     • Use secure key storage (Keystore/Keychain)            │
│     • Never hardcode credentials                            │
│     • Use environment variables for secrets                 │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

