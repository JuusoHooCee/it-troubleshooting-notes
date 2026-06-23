# Issue: Computer cannot join domain

## Problem
Computer fails to join domain with error:
"The specified domain could not be found"

---

## Cause
DNS server was not pointing to the domain controller.

---

## Solution
Set client DNS to the domain controller's IP address.

---

## Notes
- DNS is critical for Active Directory
- Without proper DNS, domain operations fail


