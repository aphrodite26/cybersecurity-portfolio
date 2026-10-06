# Network Traffic Analysis

## Overview

This project contains network traffic analysis activities completed as part of the Google Cybersecurity Professional Certificate.

The objective was to analyze network traffic, investigate security incidents, identify affected protocols and services, and understand how network attacks can impact systems and users.

---

## 1. DNS Service Incident

### Scenario

Users were unable to access a website and received a "destination port unreachable" error.

### Analysis

Network traffic captured with tcpdump showed that:

- UDP was used to send DNS requests.
- DNS traffic was directed to port 53.
- ICMP responses returned a "udp port 53 unreachable" error.
- The DNS service was not responding as expected.
- Further investigation was required to determine whether the DNS server was unavailable or whether port 53 was being blocked.

### Tools & Concepts

`tcpdump` `DNS` `UDP` `ICMP` `Port 53` `TCP/IP`

---

## 2. SYN Flood / DoS Incident

### Scenario

A web server became unavailable and users experienced connection timeout errors. Network traffic showed a large number of TCP SYN requests being sent to the server.

### Analysis

The incident was identified as a SYN flood, a type of Denial-of-Service (DoS) attack.

The attacker generated a large number of SYN requests without completing the TCP three-way handshake. This caused the server to reserve resources for incomplete connections, eventually preventing legitimate users from establishing new connections.

### Tools & Concepts

`Wireshark` `TCP` `TCP Three-Way Handshake` `SYN Flood` `DoS` `Network Monitoring`

---

## Skills Demonstrated

- Network traffic analysis
- Packet and log analysis
- Network protocol analysis
- Incident investigation
- DNS troubleshooting
- TCP/IP fundamentals
- DoS attack analysis
- Network security monitoring


