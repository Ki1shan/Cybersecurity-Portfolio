# Network Traffic Analysis (Wireshark)

## Objective
To analyze captured network traffic using Wireshark in order to identify protocols, inspect packet flows and detect potential suspicious or malicious activity.

## Methodology
- Captured network traffic using packet capture tools
- Analyzed PCAP files using Wireshark
- Applied protocol-based filters to inspect specific traffic
- Examined packet details, streams and communication patterns

## Analysis Performed

### Protocol Inspection
- Identified key protocols:
  - TCP
  - HTTP
  - DNS
- Used filters such as:
  - http
  - dns
  - tcp

### Packet Analysis
- Inspected individual packets for source/destination IPs
- Analyzed TCP handshake and communication flows
- Reviewed DNS queries for domain resolution behavior

### Stream Analysis
- Followed TCP streams to understand full communication sessions
- Observed request-response behavior in HTTP traffic

## Key Findings
- Multiple active network communications identified across TCP, HTTP and DNS protocols
- DNS queries revealed domain resolution activity which can be used for reconnaissance
- HTTP traffic observed without encryption, indicating potential data exposure
- Packet-level inspection provided visibility into communication patterns

## Security Analysis
- Unencrypted HTTP traffic can expose sensitive information to attackers
- DNS traffic can be abused for data exfiltration or reconnaissance
- Traffic analysis is essential for detecting anomalies and potential intrusions
- Monitoring network traffic helps identify suspicious behavior early

## Conclusion
The traffic analysis successfully identified active protocols and communication patterns within the network. This demonstrates the importance of packet inspection and monitoring in identifying potential security risks.

## Tools Used
- Wireshark
- TCPDump (for capture)

## Files Included
- traffic.pcapng
- traffic1.pcapng

## Note
Due to file size constraints, only relevant captures are included. Full capture data can be provided upon request.
