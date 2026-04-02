# Firewall Hardening (UFW & Windows Firewall)

## Objective
To enhance system security by restricting insecure network services and validating firewall configurations across Linux and Windows environments.

## Methodology

### Linux (Kali - UFW)
- Enabled firewall using UFW
- Denied Telnet service (port 23)
- Verified rule enforcement using telnet connection testing

### Windows Firewall
- Configured inbound rules to block Telnet (port 23)
- Managed firewall rules through Windows Defender Firewall
- Verified rule status and enforcement

## Implementation

### UFW Commands Used
- sudo ufw enable
- sudo ufw status numbered
- sudo ufw deny 23
- sudo ufw allow 22
- sudo ufw delete deny 23

### Validation
- Attempted connection using:
  - `telnet localhost 23`
- Result:
  - Connection refused → Firewall rule successfully enforced

## Key Findings
- Telnet (port 23) was successfully blocked in both environments
- Firewall rules effectively prevented unauthorized access
- Secure service (SSH - port 22) remained accessible

## Security Analysis
- Telnet transmits data in plaintext → highly insecure
- Blocking Telnet reduces risk of credential theft and unauthorized access
- Proper firewall configuration is essential for minimizing attack surface

## Conclusion
Firewall hardening was successfully implemented by blocking insecure services and validating access restrictions. This demonstrates effective defensive security practices in real-world environments.

## Tools Used
- UFW (Uncomplicated Firewall)
- Windows Defender Firewall
- Telnet (for testing)
