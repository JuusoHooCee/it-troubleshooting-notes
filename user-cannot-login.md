# Issue: User cannot login to workstation

## Problem
User receives error:
"The sign-in method you're trying to use isn't allowed"

---

## Cause
User account not allowed to log in locally or missing permissions.

---

## Solution
Check:

1. Local Security Policy:
   - Allow log on locally
2. Group membership:
   - User part of correct groups

---

## Notes
- Often happens with restricted environments
- Group Policy can override local settings
