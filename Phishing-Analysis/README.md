# Phishing Email Analysis

## Objective
To analyze phishing emails by examining email headers, sender details, embedded links and social engineering techniques to identify malicious intent and indicators of compromise.

## Methodology
- Collected suspicious phishing emails
- Analyzed email headers (Message-ID, Return-Path, Received fields)
- Inspected sender domains and reply-to addresses
- Investigated embedded URLs for legitimacy
- Identified social engineering tactics used to manipulate users

## Case Studies

### 1. Wells Fargo Phishing Email

#### Key Findings
- Fake sender: support@wellsfargo-support.net
- Suspicious domain: cabinetkignima.com
- Email originated from shadyhosting.biz :contentReference[oaicite:0]{index=0}
- Used HTTP instead of HTTPS

#### Indicators of Phishing
- Domain mismatch (not official Wells Fargo domain)
- Urgency tactic: “Security key expired”
- Grammar mistakes and inconsistent branding
- Suspicious reply-to address
- Generic greeting used

---

### 2. Microsoft Account Phishing Email

#### Key Findings
- Fake sender: no-reply.msteam2@outlook.com
- Email originated from mail.scamhost.net :contentReference[oaicite:1]{index=1}
- Invalid IP address used (293.x.x.x)
- Phishing kit identified in header (X-Mailer)

#### Indicators of Phishing
- Use of free email domain instead of official Microsoft domain
- Fake support phone number
- Urgent security alert message
- Suspicious reply-to domain
- Hidden malicious link in CTA

---

## Security Analysis
- Attackers use domain spoofing to mimic trusted brands
- Social engineering tactics (urgency, fear) are used to manipulate victims
- Malicious links redirect users to credential harvesting sites
- Header analysis helps trace the origin of phishing emails

## Conclusion
The analysis identified multiple phishing indicators including spoofed domains, malicious links, and social engineering techniques. Proper email inspection and awareness can prevent credential theft and account compromise.

## Tools Used
- MessageHeader Analyzer
- URLVoid
- IPVoid
