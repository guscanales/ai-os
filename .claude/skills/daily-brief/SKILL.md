---
name: daily-brief
description: "Prepare three priorities, due tasks and today's workout. Trigger phrases: daily brief, plan my day, morning brief."
---

# daily-brief

## Reads

Tasks.md; Areas/Health/Training Program.md; Areas/Health/Workout Log.md; Areas/Health/Sleep.md; Areas/Learning/Study Plan.md; the latest weekly review

## Writes

Command Center.md, generated Daily brief section only

## Steps

1. Read CLAUDE.md and the listed files. Confirm the date and local timezone. Use 2026-11-22 for a frozen demo run.

2. Pick at most three priorities from existing tasks. Prefer overdue work, upcoming deadlines and This Week. Do not create a duplicate task.

3. List due and overdue tasks separately, using their dates. Derive the workout from the weekday split. On a rest day, say rest day.

4. Add one brief nudge from a documented drift, such as short sleep or missed study. Do not infer a diagnosis.

5. Refresh only the Daily brief section of Command Center.md through this playbook. If file access is unavailable, return the section with its path for Gus to paste.

## Output example

2026-11-23 priorities: interview practice, spending review, recording preparation. Workout: Pull. Nudge: end editing at 22:00.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
