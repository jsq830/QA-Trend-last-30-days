---
name: test-skill
description: Use when the user wants to verify that a Codex skill repository is wired correctly by running a tiny deterministic test workflow.
---

# Test Skill

Use this skill only for repository wiring checks and smoke tests.

## Workflow

1. Confirm the skill was loaded by saying `test-skill loaded`.
2. Echo the user's requested test label if one is provided.
3. Return exactly one short next step that would prove the surrounding repo workflow works, such as committing or running validation.

Keep the response concise. Do not perform unrelated analysis.
