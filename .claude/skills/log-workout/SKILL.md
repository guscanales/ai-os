---
name: log-workout
description: "Record exercise results and apply the clean-rep progression rule. Trigger phrases: I did pull day, log workout, record my training."
---

# log-workout

## Reads

Areas/Health/Training Program.md; Areas/Health/Workout Log.md

## Writes

Areas/Health/Workout Log.md; Areas/Health/Training Program.md

## Steps

1. Read CLAUDE.md and the program. Extract date, session, exercise, actual reps per set, weight, form and last-set RIR from the message.

2. Ask for missing details needed for progression. Append the reported session even if progression cannot yet be decided. Check for an existing session on that date before appending.

3. Add the session summary and exercise details to the log. Never convert a reported estimate into a precise measurement.

4. Add 5 lb to the next target only when all prescribed reps were completed with clean form and last-set RIR 1 to 2. Use the program's per-hand rule for dumbbells. Hold weights when reps, form or effort evidence is missing.

5. Update only qualifying exercise weights in the program. Report current performance and next target separately. Flag pain without diagnosing it.

## Output example

Cable row: four sets of 10 at 85 lb, clean, RIR 2. Logged 2026-11-16. Next target: 90 lb. Pulldown held at 100 lb after a missed rep.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
