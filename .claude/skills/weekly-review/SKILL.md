---
name: weekly-review
description: "Summarize the week in one page. Trigger phrases: weekly review, review my week, Sunday review."
---

# weekly-review

## Reads

Tasks.md; Areas/Health/Workout Log.md; Areas/Health/Body Metrics.md; Areas/Money/Budget.md; Areas/Money/Spending/*.md; Areas/Learning/Study Plan.md; the last weekly review

## Writes

Areas/Journal/Weekly Reviews/YYYY-Www.md; Tasks.md if a rollover is approved; Command Center.md

## Steps

1. Read CLAUDE.md and the listed sources. Use the real run date and ISO week number. For the demo, use 2026-11-22 unless Gus requests another date.

2. Count sessions and study hours for the same Monday to Sunday period. Label money figures month to date. Preserve historical review numbers. If completed task history is missing, report unknown rather than invent a count.

3. Write Wins, What's drifting, Numbers and One change for next week. Follow Templates/Weekly Review.md. Keep it under about 500 words, at most one page.

4. Propose rollover choices before moving tasks. This Week has at most seven tasks. Move each task once and preserve its wording and tags.

5. Refresh the generated Command Center from sources. Update the review link, week heading and due-soon cutoff to the following Monday. Preserve other dashboard sections. Show changed paths.

## Output example

Weekly review saved to Areas/Journal/Weekly Reviews/2026-W47.md. Workouts: 3/4. Study: 5/6 hours. One change: record in one simple session.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
