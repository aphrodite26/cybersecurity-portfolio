# Malware Investigation Using VirusTotal and the Pyramid of Pain

## Overview

This lab is part of the Google Cybersecurity Professional Certificate and focuses on investigating a suspicious file using VirusTotal and organizing indicators of compromise (IoCs) according to the Pyramid of Pain framework.

The objective was to evaluate whether a suspicious file was malicious, examine threat intelligence findings, and identify indicators associated with potential malware activity.

## Investigation Scenario

As a Level 1 Security Operations Center (SOC) analyst at a financial services organization, I investigated an alert involving a suspicious file downloaded onto an employee's computer.

The employee received an email containing a password-protected spreadsheet attachment. After downloading and opening the file, a malicious payload executed, resulting in the creation of unauthorized executable files.

An intrusion detection system (IDS) subsequently generated an alert.

### Incident Timeline

| Time | Event |
|---|---|
| 1:11 PM | Employee received an email containing an attachment |
| 1:13 PM | Employee downloaded and opened the file |
| 1:15 PM | Multiple unauthorized executable files were created |
| 1:20 PM | IDS detected the suspicious executables and generated an alert |

## Tools and Frameworks

- VirusTotal
- SHA-256 File Hash Analysis
- Threat Intelligence
- Indicators of Compromise (IoCs)
- Pyramid of Pain
- MITRE ATT&CK Concepts

## Practical Investigation

### 1. Investigating the Suspicious File

The investigation began with the following SHA-256 hash:

```text
54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b
```

The hash was used to investigate the file through VirusTotal and review available security intelligence.

The investigation focused on four VirusTotal sections:

- **Detection:** Security vendor classifications and detection results.
- **Details:** File metadata and additional cryptographic hashes.
- **Relations:** Associated IP addresses, domains, and network connections.
- **Behavior:** Observed malware activity, including network communications, host artifacts, and tactics or techniques.

### 2. Malware Identification

The investigation findings indicated that the file was malicious.

More than 50 security vendors reportedly classified the file as malicious.

The malware was identified as **Flagpro**, which has been associated with the threat actor **BlackTech**.

These findings supported the assessment that the suspicious attachment represented a security threat.

### 3. Identifying Indicators of Compromise

The investigation documented the following indicators and behavioral findings:

| IoC Category | Investigation Finding |
|---|---|
| File Hash | `287d612e29b71c90aa54947313810a25` |
| IP Address | `207.148.109.242` |
| Domain Name | `org.misecure.com` |
| Network/Host Artifacts | HTTP requests |
| Tools/Behavior | Input capture |
| Tactics, Techniques, and Procedures | Command and Control |

These findings were organized using the Pyramid of Pain framework to illustrate different categories of threat indicators.

### 4. Applying the Pyramid of Pain

The Pyramid of Pain helps security analysts understand how difficult it may be for attackers to adapt when particular indicators or behaviors are detected and blocked.

The framework categorizes indicators into six levels:

1. Hash Values
2. IP Addresses
3. Domain Names
4. Network/Host Artifacts
5. Tools
6. Tactics, Techniques, and Procedures (TTPs)

Lower-level indicators, such as file hashes, are generally easier for attackers to change.

Higher-level indicators, particularly TTPs, are more difficult to modify because they reflect how an attacker operates.

This framework helps security teams prioritize detection strategies beyond individual file signatures.

## Security Relevance

VirusTotal and the Pyramid of Pain are useful in SOC investigations because they help analysts:

- Investigate suspicious files using threat intelligence.
- Correlate file hashes with known malware detections.
- Identify potentially malicious IP addresses and domains.
- Examine malware behavior and associated artifacts.
- Understand attacker tactics and techniques.
- Support incident triage and threat identification.
- Develop a broader understanding of detection and response strategies.

VirusTotal findings should be interpreted alongside other evidence, since individual detection results and reputation scores are not conclusive on their own.

## Skills Demonstrated

- Malware Investigation
- VirusTotal Threat Intelligence Analysis
- SHA-256 Hash Investigation
- Indicator of Compromise Identification
- Pyramid of Pain Classification
- Malware Behavior Analysis
- Security Alert Investigation
- SOC Level 1 Incident Triage

## Investigation Report

[View Investigation Findings (PDF)](Investigation-findings.pdf)

The report documents the malware assessment and the indicators identified during the investigation.

## Conclusion

This lab provided practical experience investigating a suspicious file using VirusTotal and organizing threat intelligence findings through the Pyramid of Pain.

It strengthened foundational SOC analysis skills, particularly malware identification, indicator analysis, and understanding how different types of threat intelligence contribute to security investigations.

---

**Course:** Google Cybersecurity Professional Certificate

**Activity:** Analyze an Artifact Using VirusTotal and the Pyramid of Pain
