# Network Traffic Analysis – DNS Incident

## Overview

This project was completed as part of the Google Cybersecurity Professional Certificate.

The objective was to analyze network traffic captured with tcpdump and investigate a network incident that prevented users from accessing a website.

## Scenario

Users reported receiving a "destination port unreachable" error when attempting to access a website. Network traffic was analyzed to identify the affected protocol and determine the possible cause of the incident.

## Analysis

The tcpdump logs showed that:

- UDP was used to send DNS requests.
- DNS traffic was directed to port 53.
- ICMP responses returned a "udp port 53 unreachable" error.
- The traffic indicated that the DNS service was not responding as expected.
- Further investigation was required to determine whether the DNS server was unavailable or whether traffic to port 53 was being blocked.

## Skills Demonstrated

- Network traffic analysis
- tcpdump log analysis
- DNS and UDP traffic analysis
- ICMP error interpretation
- Network troubleshooting
- Incident analysis

## Tools & Technologies

`tcpdump` `DNS` `UDP` `ICMP` `TCP/IP`
