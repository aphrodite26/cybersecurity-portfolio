# Network Traffic Capture and Analysis with tcpdump

## Overview

This lab focuses on capturing, filtering, and analyzing network traffic using `tcpdump`, a command-line packet analyzer commonly used in Linux environments.

The objective was to understand how network packets can be captured from a network interface, saved to a PCAP file, and examined to identify communication between systems.

## Tools and Technologies

- Linux
- Bash Shell
- tcpdump
- TCP/IP
- HTTP
- PCAP Files

## Lab Objectives

- Identify available network interfaces.
- Capture network traffic using `tcpdump`.
- Apply packet capture filters.
- Save captured packets to a PCAP file.
- Read and analyze previously captured network traffic.
- Examine packet headers and payload information.

## Practical Activities

### 1. Identifying Network Interfaces

Used `tcpdump` to identify network interfaces available for packet capture.

```bash
sudo tcpdump -D
```

This command lists interfaces that can be used to capture network traffic.

### 2. Capturing Network Traffic

Captured packets from a network interface using `tcpdump`.

Example:

```bash
sudo tcpdump -i eth0
```

The `-i` option specifies the network interface.

This allows network traffic to be observed directly from the Linux terminal.

### 3. Filtering HTTP Traffic

Applied a port-based capture filter to focus on HTTP traffic.

```bash
sudo tcpdump -i eth0 port 80
```

This command captures packets associated with TCP or UDP port 80.

Filtering helps reduce unrelated network traffic and focus on specific communications.

### 4. Saving Captured Packets

Saved network traffic to a PCAP file for later analysis.

```bash
sudo tcpdump -i eth0 -w capture.pcap
```

The `-w` option writes captured packets to a file instead of displaying them directly in the terminal.

PCAP files can be examined using tools such as tcpdump and Wireshark.

### 5. Reading Captured Traffic

Read previously captured network packets from a PCAP file.

```bash
sudo tcpdump -r capture.pcap
```

The `-r` option reads packets from a saved capture file.

This allows analysts to investigate network traffic after the capture has finished.

### 6. Inspecting Packet Contents

Used additional options to display more detailed packet information.

```bash
sudo tcpdump -r capture.pcap -v
```

The `-v` option increases the amount of packet information displayed.

To examine packet contents in hexadecimal and ASCII formats:

```bash
sudo tcpdump -r capture.pcap -X
```

The `-X` option displays packet data in hexadecimal and ASCII representations.

These options can help analysts examine packet headers, network protocols, and readable packet contents.

## Security Relevance

Packet capture and analysis are important activities in cybersecurity monitoring and incident investigation.

Security analysts can use `tcpdump` to:

- Investigate suspicious network communications.
- Identify unexpected connections between systems.
- Examine traffic associated with specific ports.
- Capture evidence during incident investigations.
- Analyze network protocols and packet metadata.
- Save network traffic for further examination in Wireshark.

## Skills Demonstrated

- Linux Command-Line Operations
- Network Traffic Capture
- tcpdump Packet Filtering
- TCP/IP Traffic Analysis
- PCAP File Analysis
- Packet Header Inspection
- Network Security Monitoring

## Conclusion

This lab provided practical exposure to network traffic capture and analysis using tcpdump in a Linux environment.

It strengthened command-line network investigation skills and demonstrated how packet capture tools can support security monitoring and incident response.

---

**Course:** Google Cybersecurity Professional Certificate

**Lab:** Capture and Analyze Network Traffic with tcpdump
