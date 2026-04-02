# Network Scanning (Nmap)

## Objective
To perform network reconnaissance using TCP SYN scanning across NAT and Bridged environments to identify active hosts, open ports and exposed services.

## Methodology
- Tool Used: Nmap
- Scan Type: TCP SYN Scan (-sS)
- Networks Scanned:
  - NAT Network: 10.0.2.0/24
  - Bridged Network: 192.168.1.0/24

## Key Findings

### NAT Network Results
- Host: 10.0.2.2
  - 135/tcp – MSRPC
  - 445/tcp – SMB
  - 3306/tcp – MySQL
  - 9080/tcp – Web Service

- Host: 10.0.2.3
  - 53/tcp – DNS

### Bridged Network Results
- Host: 192.168.1.1
  - 53/tcp – DNS
  - 80/tcp – HTTP
  - 443/tcp – HTTPS

- Host: 192.168.1.9
  - 135/tcp – MSRPC
  - 139/tcp – NetBIOS
  - 445/tcp – SMB
  - 3306/tcp – MySQL

## Security Analysis
- SMB (Port 445) → susceptible to lateral movement and exploitation
- MySQL (Port 3306) → risk of unauthorized database access if not secured
- HTTP (Port 80) → unencrypted communication, vulnerable to interception
- DNS (Port 53) → can be abused for reconnaissance or DNS-based attacks

## Conclusion
The scan successfully identified multiple active hosts and exposed services across both NAT and Bridged networks, highlighting potential attack surfaces that require further security assessment and hardening.

## Tools Used
- Nmap
- Wireshark (for traffic analysis)

## Files Included
- nat_scan.txt
- nat_scan.xml
- bridged_scan.txt
- nmap_scan.pcapng
