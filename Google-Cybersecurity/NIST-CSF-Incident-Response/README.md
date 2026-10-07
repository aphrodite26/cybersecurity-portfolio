# NIST Cybersecurity Framework – Incident Response

## Overview

This project was completed as part of the Google Cybersecurity Professional Certificate.

The objective was to analyze a network security incident and apply the NIST Cybersecurity Framework (CSF) to develop a structured approach for identifying, protecting against, detecting, responding to, and recovering from cybersecurity incidents.

## Incident Scenario

A multimedia company experienced a denial-of-service attack caused by a flood of incoming ICMP packets.

The attack overwhelmed the internal network and caused network services to stop responding. The incident was traced to a malicious actor who was able to send large amounts of ICMP traffic through an improperly configured firewall.

## NIST CSF Analysis

### Identify

The incident was identified as an ICMP flood attack affecting the organization's internal network and critical network resources.

### Protect

Security controls were implemented to reduce the risk of similar attacks:

- Firewall rules to limit incoming ICMP traffic.
- IDS/IPS filtering based on suspicious ICMP traffic characteristics.

### Detect

Detection capabilities included:

- Source IP address verification to identify spoofed addresses.
- Network monitoring software to detect abnormal traffic patterns.

### Respond

The response strategy included:

- Isolating affected systems.
- Restoring critical systems and services.
- Analyzing network logs for suspicious activity.
- Reporting incidents to management and appropriate authorities when necessary.

### Recover

Recovery procedures included:

- Blocking malicious ICMP traffic.
- Taking non-critical services offline to reduce network traffic.
- Restoring critical services first.
- Returning non-critical systems and services to normal operation after the attack was contained.

## Skills Demonstrated

- NIST Cybersecurity Framework (CSF)
- Incident response
- DoS / ICMP flood analysis
- Network security monitoring
- Firewall security
- IDS/IPS
- Incident documentation
- Security controls assessment
- Recovery planning

## Framework

`Identify` → `Protect` → `Detect` → `Respond` → `Recover`

## Project File

- [NIST CSF Incident Report](./NIST-CSF-Incident-Report.pdf)
