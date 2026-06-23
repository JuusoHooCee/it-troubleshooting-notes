# Issue: Network drive not mapping

## Problem
Mapped drive does not appear after login.

---

## Cause
GPO not applied or incorrect path.

---

## Solution
Check:

1. Run:
   gpupdate /force

2. Verify GPO is applied:
   gpresult /r

3. Confirm share path is correct:
   \\server\share

---

## Notes
- GPO processing order matters
- Network delays can sometimes affect mapping
