# Working Rules

## What to write

Define the operational and engineering expectations that should always apply.

## Why it matters

Rules reduce friction and make collaboration more predictable.

## Example

### Always

- Use type hints where the language supports them
- Explain architecture changes before implementation
- Prefer readable code over clever shortcuts
- Write tests for critical business logic
- Never expose secrets or credentials
- Keep documentation aligned with implementation

### Never

- Commit directly to production without review
- Delete migrations without a replacement plan
- Skip error handling for user-facing flows
- Ship features without basic validation

---

# Review Expectations

## What to write

State how work should be reviewed and validated.

## Why it matters

Clear review norms improve quality and reduce rework.

## Example

- PRs should include a summary, tests, and risk notes
- Reviewers should focus on correctness, security, and maintainability
- Large changes should include a short design note
