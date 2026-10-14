---
'e2e': patch
'@e2e-dev/mobile': patch
---

The mobile engine now bounds reads (snapshots and screenshots) by their operation budget so a hung device does not hold the step until the test timeout. The locator poll measures how long reads take and grants the last read extra time past the deadline so a slow read still finishes, avoiding timeouts when elements appear late.
