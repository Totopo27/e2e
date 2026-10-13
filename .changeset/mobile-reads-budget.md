---
'e2e': patch
'@e2e-dev/mobile': patch
---

Bound mobile reads (snapshots and screenshots) by their operation budget without cutting off a slow last poll into a timeout. Engines may now declare an estimated `readLatency` in milliseconds (the mobile engine sets 2,000 ms), which poll loops and `pollCondition` grant past the deadline to distinguish a slow read from a hung one.
