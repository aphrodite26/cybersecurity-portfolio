# Network Hardening

## Overview

This project was completed as part of the Google Cybersecurity Professional Certificate.

The objective was to investigate a website security incident, analyze network traffic using tcpdump, identify the attack that led to the compromise, and recommend security measures to reduce the risk of similar attacks.

## Incident Scenario

A website was compromised after an attacker gained access to an administrative account through a brute-force attack.

The attacker modified the website's source code and added malicious JavaScript that prompted visitors to download an executable file. After executing the file, users were redirected to a malicious website.

## Network Analysis

The incident was investigated in a sandbox environment using tcpdump.

The analysis identified:

- DNS requests used to resolve the website domains.
- HTTP traffic used to communicate with the web servers.
- HTTP traffic associated with the malicious file download.
- Network traffic redirecting users from the legitimate website to a malicious website.

## Security Findings

The investigation determined that:

- The administrative account was using a default password.
- There were insufficient controls to prevent brute-force login attempts.
- The attacker gained administrative access and modified the website.
- Users were exposed to a malicious file and website redirect.

## Hardening Recommendations

Security measures that can reduce the risk of similar attacks include:

- Replacing default passwords with strong passwords.
- Implementing multi-factor authentication (MFA/2FA).
- Limiting failed login attempts.
- Monitoring authentication attempts.
- Preventing reuse of previous or default passwords.

## Skills Demonstrated

- Network hardening
- tcpdump traffic analysis
- HTTP and DNS analysis
- Brute-force attack investigation
- Web security incident analysis
- Security control recommendations
- Incident documentation

## Tools & Concepts

`tcpdump` `HTTP` `DNS` `TCP/IP` `Brute Force` `MFA` `Network Hardening`
