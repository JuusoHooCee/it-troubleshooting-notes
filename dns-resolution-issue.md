# Issue: Cannot access internal network resources

## Problem
Users cannot access network shares or internal services using hostname.

Example:
\\fileserver → not working  
\\192.168.1.10 → working

---

## Cause
DNS resolution failure. Client was not using the correct DNS server.

---

## Solution
Set the correct DNS server (Domain Controller IP) on the client.

Steps:
1. Open network adapter settings
2. Change DNS server to domain controller IP
3. Run:
   ipconfig /flushdns

---

## Notes
- Active Directory relies heavily on DNS
- Incorrect DNS breaks domain functionality
