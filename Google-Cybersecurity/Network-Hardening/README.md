# Network Hardening

## Overview

This project contains network hardening and security analysis activities completed as part of the Google Cybersecurity Professional Certificate.

The activities focus on investigating network security incidents, identifying vulnerabilities, analyzing network traffic, and recommending security controls to reduce the risk of future attacks.

---

## 1. Web Server Security Incident

### Scenario

A website was compromised after an attacker gained access to an administrative account through a brute-force attack.

The attacker modified the website's source code and added malicious JavaScript that prompted users to download a malicious executable file and redirected them to a fake website.

### Network Analysis

The incident was investigated in a sandbox environment using tcpdump.

The analysis identified:

- DNS requests used to resolve website domains.
- HTTP traffic between the client and web servers.
- HTTP traffic associated with the malicious file download.
- Traffic redirecting users from the legitimate website to a malicious website.

### Security Findings

The investigation identified several security issues:

- The administrative account was using a default password.
- Controls to prevent brute-force attacks were insufficient.
- The attacker gained administrative access and modified the website.
- Users were exposed to a malicious file and website redirect.

### Recommended Hardening

Potential security improvements included:

- Replacing default passwords.
- Implementing multi-factor authentication (MFA).
- Limiting failed login attempts.
- Monitoring authentication attempts.
- Strengthening password management practices.

---

## 2. Security Risk Assessment

### Scenario

A social media organization experienced a data breach that exposed customer information. A security assessment identified weaknesses in authentication and network security controls.

### Identified Vulnerabilities

- Employees were sharing passwords.
- The database administrator account used a default password.
- Firewall rules were not configured to properly filter network traffic.
- Multi-factor authentication was not implemented.

### Hardening Recommendations

Three security hardening measures were selected:

**Multi-Factor Authentication (MFA)**  
Adds an additional authentication layer beyond passwords and reduces the risk of unauthorized access.

**Strong Password Policies**  
Password requirements, restrictions on password reuse, and controls for repeated failed login attempts can reduce the risk of password-based attacks.

**Regular Firewall Maintenance**  
Firewall rules should be regularly reviewed and updated to control allowed and denied network traffic and respond to emerging security threats.

---

## Skills Demonstrated

- Network hardening
- Security risk assessment
- Network traffic analysis
- tcpdump analysis
- HTTP and DNS analysis
- Brute-force attack investigation
- Authentication security
- Firewall security
- Security control recommendations
- Incident documentation

## Tools & Concepts

`tcpdump` `HTTP` `DNS` `TCP/IP` `MFA` `Firewall` `Password Policies` `Brute Force` `Network Hardening`
