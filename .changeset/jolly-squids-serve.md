---
'e2e': patch
---

A replayed step's end check now waits out the larger of the recorded end wait and the configured assertion timeout, so steps replaying under load do not fail with `end-mismatch` before slow end states arrive.

