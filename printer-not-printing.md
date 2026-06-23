# Issue: Printer not printing

## Problem
User sends print job but nothing prints.

Print queue shows stuck jobs.

---

## Cause
Print spooler service was stuck.

---

## Solution
Restart the print spooler service:

1. Open Services
2. Find "Print Spooler"
3. Restart service

OR via command line:
net stop spooler
net start spooler

---

## Notes
- Common issue in shared printers
- Restarting spooler often resolves queue problems
