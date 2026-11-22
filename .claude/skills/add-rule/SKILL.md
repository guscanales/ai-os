---
name: add-rule
description: "Save a durable correction in the shared rules file. Trigger phrases: remember this correction, add a rule, stop doing that."
---

# add-rule

## Reads

CLAUDE.md Lessons learned; the user correction and its context

## Writes

CLAUDE.md Lessons learned only

## Steps

1. Read CLAUDE.md and the actual correction. Capture what Gus wants done differently without adding a broader restriction.

2. Check for an existing equivalent lesson. Update it when clarified rather than adding conflicting duplicates.

3. Append one short line under Lessons learned using YYYY-MM-DD: correction. Use the actual run date, or 2026-11-22 for a requested demo run.

4. Never copy secrets or private identifiers into a rule. If the correction conflicts with a higher-priority instruction, explain the limit instead of promising compliance.

5. Report the exact saved line. Keep AGENTS.md as a three-line pointer.

## Output example

2026-11-22: Label partial-month spending before comparing it with a full monthly budget.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
