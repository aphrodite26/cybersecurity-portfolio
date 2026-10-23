# Wireshark Packet Analysis Lab

## Overview

This lab is part of the Google Cybersecurity Professional Certificate and focuses on inspecting network traffic using Wireshark, a graphical network protocol analyzer.

The objective was to examine a sample packet capture (`.pcap`) file, identify network communication details, and apply display filters to investigate specific packets and protocols.

## Tools and Technologies

- Wireshark
- Windows Virtual Machine
- Packet Capture (PCAP) Files
- TCP/IP Networking
- DNS, TCP, UDP, HTTP, and ICMP

## Lab Objectives

- Inspect network packets using Wireshark.
- Identify source and destination IP addresses.
- Examine Ethernet, IPv4, and TCP packet headers.
- Apply display filters to isolate relevant network traffic.
- Analyze DNS queries and responses.
- Identify HTTP traffic and search TCP packet payloads.

## Practical Activities

### 1. Exploring Packet Capture Data

Opened a sample `.pcap` file in Wireshark and examined the packet list.

Reviewed packet information including:

- Packet number and timestamp
- Source and destination IP addresses
- Network protocols
- Packet length
- Packet information and protocol details

Explored how Wireshark uses packet coloring rules to distinguish different types of network traffic.

### 2. Filtering Traffic by IP Address

Used Wireshark display filters to isolate traffic associated with a specific IP address.

```text
ip.addr == 142.250.1.139
```

Examined individual packets to identify their protocol layers, including Ethernet II, IPv4, and TCP.

### 3. Analyzing Source, Destination, and MAC Addresses

Applied filters to identify traffic originating from or directed toward a specific IP address.

**Source IP filter:**

```text
ip.src == 142.250.1.139
```

**Destination IP filter:**

```text
ip.dst == 142.250.1.139
```

**MAC address filter:**

```text
eth.addr == 42:01:ac:15:e0:02
```

These filters helped distinguish incoming and outgoing network traffic and examine communication between network devices.

### 4. Investigating DNS Traffic

Filtered DNS traffic using UDP port 53.

```text
udp.port == 53
```

Inspected DNS queries and responses associated with:

```text
opensource.google.com
```

Examined how DNS resolves domain names into IP addresses and how this information appears in captured packets.

### 5. Inspecting HTTP and TCP Traffic

Filtered HTTP-related traffic using TCP port 80.

```text
tcp.port == 80
```

Examined packet properties including:

- Source and destination addresses
- TCP ports
- Time to Live (TTL)
- IP header length
- Frame length
- TCP flags

Also searched TCP packet data for a specific text string:

```text
tcp contains "curl"
```

This demonstrated how Wireshark can identify packets containing particular application-related content.

## Security Relevance

Network packet analysis is an important skill for Security Operations Center (SOC) analysts.

Wireshark can support security investigations by helping analysts:

- Identify suspicious network connections.
- Investigate unexpected DNS requests.
- Examine communication between hosts.
- Analyze network protocols and packet metadata.
- Filter large packet captures to focus on relevant traffic.
- Investigate potential indicators of compromise.

## Skills Demonstrated

- Network Traffic Analysis
- Packet Inspection
- Wireshark Display Filtering
- TCP/IP Protocol Analysis
- DNS Traffic Analysis
- HTTP Traffic Inspection
- Basic Network Security Investigation

## Conclusion

This lab provided practical experience using Wireshark to inspect packet capture files, apply network traffic filters, and analyze communication between systems.

It strengthened foundational network analysis skills relevant to cybersecurity monitoring and incident investigation.

---

**Course:** Google Cybersecurity Professional Certificate

**Lab:** Analyze Network Traffic with Wireshark
