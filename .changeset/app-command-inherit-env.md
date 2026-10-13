---
'e2e': minor
---

Support passing host environment variables through to `app.command` without listing them in the committed config via `app.command.inheritEnv` in config and the `E2E_APP_INHERIT_ENV` environment variable (comma-separated list of variable names or trailing `*` patterns).
