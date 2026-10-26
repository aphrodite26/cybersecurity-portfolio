# Phishing Alert Investigation & Escalation

## Project Overview

This project documents a phishing alert investigation conducted as part of the Google Cybersecurity Professional Certificate.

Acting as a Level 1 Security Operations Center (SOC) analyst, I reviewed a suspicious email alert, analyzed indicators of phishing, evaluated a previously verified malicious file hash, and followed an incident response playbook to determine whether the alert required escalation.

## Scenario

A financial services organization received an alert indicating that an employee may have downloaded and opened a malicious email attachment.

The investigation involved reviewing the email's sender information, subject line, message content, attachment, and known malicious SHA-256 file hash.

## Alert Details

| Field | Value |
|---|---|
| Ticket ID | A-2703 |
| Alert Type | Phishing / Possible Malware Download |
| Severity | Medium |
| Suspicious Attachment | `bfsvc.exe` |
| File Hash | SHA-256 |
| Final Ticket Status | Escalated |

## Investigation Process

### 1. Alert Evaluation

Reviewed the phishing alert ticket and supporting email information to identify suspicious characteristics.

### 2. Phishing Indicators

Identified several indicators associated with a potential phishing attempt:

- Inconsistencies between the sender's identity and email address.
- Grammatical errors in the email subject and message.
- A password-protected attachment presented as a resume and cover letter.
- An executable (`.exe`) file attached to a job application email.

### 3. Malicious File Verification

Used the findings from a previous file hash investigation, which confirmed that the attachment's SHA-256 hash was associated with a known malicious file.

### 4. Incident Escalation

Followed the phishing incident response playbook to determine the appropriate action.

Based on the confirmed malicious attachment, suspicious email characteristics, and Medium alert severity, the ticket was escalated to a Level 2 SOC analyst for further investigation and response.

## Outcome

**Final Decision: Escalated**

The alert was documented with supporting evidence and an explanation of the escalation decision.

## Skills Demonstrated

- SOC Level 1 alert triage
- Phishing email analysis
- Indicators of compromise (IOC) identification
- Malicious file hash investigation
- Incident response playbook execution
- Security ticket documentation
- Incident escalation procedures

## Project Files

- [Completed Phishing Alert Ticket](Completed-alert-ticket.pdf)

---

*Completed as part of the Google Cybersecurity Professional Certificate — Sound the Alarm: Detection and Response.*
