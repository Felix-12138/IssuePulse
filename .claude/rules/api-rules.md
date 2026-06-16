---
paths:
  - "src/app/api/**/*.ts"
  - "src/server/**/*.ts"
---

# API Rules
- Validate every request body before use.
- Return consistent JSON errors: `{ error: { code, message } }`.
- Keep handlers thin; move domain logic to `src/domain/`.
- Add or update tests for non-trivial behavior.
