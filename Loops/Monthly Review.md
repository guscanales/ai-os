# Monthly Review

A loop is a saved prompt on a schedule. This file does not activate a schedule. Choose one runtime per loop to avoid duplicate writes.

| Setting | Value |
|---|---|
| When | First day of each month at 18:00, reviewing the previous month, America/Chicago |
| Reads | CLAUDE.md; Budget.md; Debt Plan.md; Spending notes; Subscriptions.md; Body Metrics.md; Study Plan.md; Job Applications.md; Goals notes; Documents & Renewals.md; Maintenance.md; weekly reviews; Tasks.md. Resolve area files by their paths in this vault. |
| Writes | Areas/Journal/Monthly Reviews/YYYY-MM.md; Command Center.md; source financial notes only via process-statements after reconciliation |

## Exact run prompt

```text
Read CLAUDE.md. Use today's date in America/Chicago and review the previous calendar month. Read Areas/Money/Budget.md, Debt Plan.md, Spending notes and Subscriptions.md; Areas/Health/Body Metrics.md; Areas/Learning/Study Plan.md; Areas/Career/Job Applications.md; Areas/Goals/; Areas/Home/Documents & Renewals.md and Maintenance.md; weekly reviews and Tasks.md. Compare spending with the monthly budget, confirmed debt changes, workouts, study hours, application progress and goal measures. Check renewals in the next 90 days. Label missing coverage and estimates. Do not close an incomplete month or invent statement reconciliation. Use process-statements only if readable redacted sources are provided. Write a short monthly review to Areas/Journal/Monthly Reviews/YYYY-MM.md, creating that folder on the first run. Include wins, drift, numbers and at most three proposed changes. Refresh Command Center.md only from verified source values. Propose actions in Tasks.md without duplication and keep This Week at seven or fewer. Ask before moving tasks, deleting, sending or buying. If files are unavailable, request fresh sources and return proposed content by path for manual saving.
```

For a demo replay, replace "today" with 2026-11-22. For real use, keep the current run date. Do not silently move the fictional records forward.

## Claude: Claude Code routine or scheduled task

In Claude Code Desktop, open this vault folder. Open Scheduled tasks, create a local task, select this folder and paste the setup below. Keep the computer awake and the app running for local tasks. A cloud routine needs its own accessible copy of the files and does not sync a local vault by itself. Test one run before enabling repeats. [Official setup](https://code.claude.com/docs/en/desktop-scheduled-tasks).

```text
Create a local scheduled task named AI OS Monthly Review. Schedule: First day of each month at 18:00, reviewing the previous month, America/Chicago. Working folder: the AI OS vault I selected. Run these instructions:
Read CLAUDE.md. Use today's date in America/Chicago and review the previous calendar month. Read Areas/Money/Budget.md, Debt Plan.md, Spending notes and Subscriptions.md; Areas/Health/Body Metrics.md; Areas/Learning/Study Plan.md; Areas/Career/Job Applications.md; Areas/Goals/; Areas/Home/Documents & Renewals.md and Maintenance.md; weekly reviews and Tasks.md. Compare spending with the monthly budget, confirmed debt changes, workouts, study hours, application progress and goal measures. Check renewals in the next 90 days. Label missing coverage and estimates. Do not close an incomplete month or invent statement reconciliation. Use process-statements only if readable redacted sources are provided. Write a short monthly review to Areas/Journal/Monthly Reviews/YYYY-MM.md, creating that folder on the first run. Include wins, drift, numbers and at most three proposed changes. Refresh Command Center.md only from verified source values. Propose actions in Tasks.md without duplication and keep This Week at seven or fewer. Ask before moving tasks, deleting, sending or buying. If files are unavailable, request fresh sources and return proposed content by path for manual saving.
```

## ChatGPT: scheduled tasks

Open Scheduled and paste the setup below. Scheduled tasks cannot read Project uploads, including when created inside that Project. Use the schedule as a reminder to open a normal conversation with fresh notes. Then paste the exact run prompt above. A normal Project chat can use its uploaded copies. Save the returned Markdown into Obsidian yourself, or use Codex with folder access. [Official task guidance](https://help.openai.com/en/articles/10291617-scheduled-tasks-in-chatgpt).

```text
Schedule AI OS Monthly Review: First day of each month at 18:00, reviewing the previous month, America/Chicago. Remind me to open my AI OS vault and run the prompt in Loops/Monthly Review.md with fresh source notes in a normal chat or Codex. List the inputs I need: CLAUDE.md; Budget.md; Debt Plan.md; Spending notes; Subscriptions.md; Body Metrics.md; Study Plan.md; Job Applications.md; Goals notes; Documents & Renewals.md; Maintenance.md; weekly reviews; Tasks.md. You cannot read my Project uploads from this scheduled task. Do not claim you reviewed or edited files. Ask me to supply fresh notes for the review.
```

## Grok: Automations

Open Automations, create a new automation and paste the setup below. Choose the named schedule and timezone. Attach only safe notes or a supported connector with the required access. Attachments are snapshots, so replace them when notes change. No local Obsidian access is assumed. Use Run now to test. Copy any proposed Markdown back manually if writing is unavailable. [Official automation guidance](https://x.ai/news/grok-automations).

```text
Create an automation named AI OS Monthly Review. Schedule: First day of each month at 18:00, reviewing the previous month, America/Chicago. Use only current notes I explicitly attach or make available through a supported connector. If their as-of dates are old, request fresh sources. Never assume access to my local vault. Run these instructions when current sources are available:
Read CLAUDE.md. Use today's date in America/Chicago and review the previous calendar month. Read Areas/Money/Budget.md, Debt Plan.md, Spending notes and Subscriptions.md; Areas/Health/Body Metrics.md; Areas/Learning/Study Plan.md; Areas/Career/Job Applications.md; Areas/Goals/; Areas/Home/Documents & Renewals.md and Maintenance.md; weekly reviews and Tasks.md. Compare spending with the monthly budget, confirmed debt changes, workouts, study hours, application progress and goal measures. Check renewals in the next 90 days. Label missing coverage and estimates. Do not close an incomplete month or invent statement reconciliation. Use process-statements only if readable redacted sources are provided. Write a short monthly review to Areas/Journal/Monthly Reviews/YYYY-MM.md, creating that folder on the first run. Include wins, drift, numbers and at most three proposed changes. Refresh Command Center.md only from verified source values. Propose actions in Tasks.md without duplication and keep This Week at seven or fewer. Ask before moving tasks, deleting, sending or buying. If files are unavailable, request fresh sources and return proposed content by path for manual saving.
```

## Plain fallback

Set an ordinary calendar reminder with the time above. Open this note and paste the exact run prompt into an AI with the listed files. Review the result, then save it at the named path. If no AI is available, use the same headings to review the source notes yourself.
