## OWASP Top 10 Learning Checklist

### A01:2021 - Broken Access Control
- [x] Path Traversal
- [x] IDOR
- [x] CORS Misconfiguration
- [x] CSRF
- [x] URL Redirection
- [x] File Inclusion (LFI/RFI)
- [ ] Forced Browsing (practice more)

### A02:2021 - Cryptographic Failures
- [x] JWT Attacks (partial)
- [ ] Weak Encryption
- [ ] Sensitive Data Exposure
- [ ] TLS/SSL Vulnerabilities
- [ ] Hardcoded Credentials

### A03:2021 - Injection
- [x] SQL Injection
- [x] OS Command Injection
- [x] XSS (DOM, Reflected, Stored)
- [x] XXE
- [x] LFI/RFI
- [ ] NoSQL Injection
- [ ] SSTI (Server-Side Template Injection)
- [ ] LDAP Injection

### A04:2021 - Insecure Design
- [x] File Upload Vulnerabilities
- [x] Race Conditions
- [x] Clickjacking
- [ ] Business Logic Flaws (practice more)

### A05:2021 - Security Misconfiguration
- [x] Information Disclosure
- [x] Host Header Attacks
- [x] CORS Misconfiguration
- [ ] Default Credentials
- [ ] Directory Listing

### A06:2021 - Vulnerable Components
- [ ] CVE Exploitation
- [ ] Outdated Libraries
- [ ] Dependency Confusion

### A07:2021 - Auth Failures
- [x] JWT Attacks
- [ ] Session Hijacking
- [ ] Session Fixation
- [ ] Brute Force (advanced)
- [ ] 2FA Bypass
- [ ] Credential Stuffing

### A08:2021 - Integrity Failures
- [ ] Insecure Deserialization
- [ ] Unsigned Updates
- [ ] CI/CD Pipeline Attacks

### A09:2021 - Logging Failures
- [ ] Log Injection
- [ ] Insufficient Logging

### A10:2021 - SSRF
- [x] Basic SSRF
- [x] Blind SSRF
- [x] SSRF to RCE
- [x] Cloud Metadata Access

### Additional Vulnerabilities Covered
- [x] WebSocket Vulnerabilities
- [x] Web LLM Attacks