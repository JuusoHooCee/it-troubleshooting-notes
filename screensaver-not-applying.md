# Issue: Screensaver not applying via GPO

## Problem
Screensaver settings are configured, but not applied to users.

---

## Cause
Incorrect GPO scope or wrong registry configuration.

---

## Solution
Check:

1. GPO linked to correct OU
2. User is inside target OU
3. Policies enabled:
   - Enable screen saver
   - Force specific screen saver
   - Password protect screen saver

4. Run:
   gpupdate /force

---

## Notes
- User Configuration vs Computer Configuration matters
- Always test with a single user first
