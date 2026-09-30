---
mode: 'agent'
model: GPT-4.1
---

# Create Scenarios

Use the project domain knowledge to create exhaustive functional test scenarios for the requested feature or full application.

Read `eventhub-domain.md` first.

Then create scenarios in `docs/test-scenarios.md` using this structure:

```markdown
### TC-<NNN>: <Title>
**Category**: <Happy Path | Business Rule | Security | Negative | Edge Case | UI State>
**Priority**: <P0 | P1 | P2 | P3>
**Preconditions**: <what must be true>
**Steps**: <numbered actions>
**Expected Results**: <what to verify>
**Business Rule**: <rule from domain skill>
**Suggested Layer**: <E2E | API | Component | Unit>
```

Apply all six lenses for every feature:
- Happy Path
- Business Rules
- Security
- Negative/Error
- Edge Cases
- UI State

The prompt/feature to cover is:

$AGENT_REQUEST
