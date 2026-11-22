---
name: people-checkin
description: "Find upcoming birthdays and late check-ins with gift ideas. Trigger phrases: who should I check in with, upcoming birthdays, people check-in."
---

# people-checkin

## Reads

Areas/People/People.md; Areas/People/Gift Ideas.md; Tasks.md

## Writes

Chat output only; People.md contact dates only after Gus confirms contact; Tasks.md only for agreed new actions

## Steps

1. Read CLAUDE.md. Use today through today plus 14 days, inclusive. Include overdue check-ins even if their date is before today.

2. Read next-occurrence birthday dates and check-in dates. List each person once, merging a birthday and overdue check-in if both apply.

3. Attach one existing gift idea and budget to each person. Suggest a simple message draft if useful. Never claim contact took place.

4. Check Tasks.md before proposing actions. Ask before sending messages or purchasing anything. Update last contact only when Gus reports an actual conversation.

5. Return dates, why each person appears and one idea each. Do not expose contact details.

## Output example

2026-11-22 to 2026-12-06: Maya, birthday 2026-11-26, sketchbook $20. Leo, birthday 2026-12-05, coffee $25. Nina, overdue since 2026-11-21, plant pot $15. Also check in with Owen, Priya and Sam on their listed dates.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
