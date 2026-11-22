# Daily Brief

A loop is a saved prompt on a schedule. This file does not activate a schedule. Choose one runtime per loop to avoid duplicate writes.

| Setting | Value |
|---|---|
| When | Daily at 07:00, America/Chicago |
| Reads | CLAUDE.md; Tasks.md; Training Program.md; Workout Log.md; Sleep.md; Study Plan.md; latest weekly review. Resolve area files by their paths in this vault. |
| Writes | Command Center.md, generated Daily brief section |

## Exact run prompt

```text
Read CLAUDE.md and .claude/skills/daily-brief/SKILL.md. Use today's date in America/Chicago. Run daily-brief from the current source notes. Return today's three priorities from existing tasks, due and overdue tasks, the workout of the day and one nudge backed by a documented drift. Refresh only the generated Daily brief section of Command Center.md. Do not add tasks or send messages. If source files are unavailable or stale, say which ones are needed and do not invent a brief. If you cannot write files, return the section and its target path for me to paste.
```

For a demo replay, replace "today" with 2026-11-22. For real use, keep the current run date. Do not silently move the fictional records forward.

## Claude: Claude Code routine or scheduled task

In Claude Code Desktop, open this vault folder. Open Scheduled tasks, create a local task, select this folder and paste the setup below. Keep the computer awake and the app running for local tasks. A cloud routine needs its own accessible copy of the files and does not sync a local vault by itself. Test one run before enabling repeats. [Official setup](https://code.claude.com/docs/en/desktop-scheduled-tasks).

```text
Create a local scheduled task named AI OS Daily Brief. Schedule: Daily at 07:00, America/Chicago. Working folder: the AI OS vault I selected. Run these instructions:
Read CLAUDE.md and .claude/skills/daily-brief/SKILL.md. Use today's date in America/Chicago. Run daily-brief from the current source notes. Return today's three priorities from existing tasks, due and overdue tasks, the workout of the day and one nudge backed by a documented drift. Refresh only the generated Daily brief section of Command Center.md. Do not add tasks or send messages. If source files are unavailable or stale, say which ones are needed and do not invent a brief. If you cannot write files, return the section and its target path for me to paste.
```

## ChatGPT: scheduled tasks

Open Scheduled and paste the setup below. Scheduled tasks cannot read Project uploads, including when created inside that Project. Use the schedule as a reminder to open a normal conversation with fresh notes. Then paste the exact run prompt above. A normal Project chat can use its uploaded copies. Save the returned Markdown into Obsidian yourself, or use Codex with folder access. [Official task guidance](https://help.openai.com/en/articles/10291617-scheduled-tasks-in-chatgpt).

```text
Schedule AI OS Daily Brief: Daily at 07:00, America/Chicago. Remind me to open my AI OS vault and run the prompt in Loops/Daily Brief.md with fresh source notes in a normal chat or Codex. List the inputs I need: CLAUDE.md; Tasks.md; Training Program.md; Workout Log.md; Sleep.md; Study Plan.md; latest weekly review. You cannot read my Project uploads from this scheduled task. Do not claim you reviewed or edited files. Ask me to supply fresh notes for the review.
```

## Grok: Automations

Open Automations, create a new automation and paste the setup below. Choose the named schedule and timezone. Attach only safe notes or a supported connector with the required access. Attachments are snapshots, so replace them when notes change. No local Obsidian access is assumed. Use Run now to test. Copy any proposed Markdown back manually if writing is unavailable. [Official automation guidance](https://x.ai/news/grok-automations).

```text
Create an automation named AI OS Daily Brief. Schedule: Daily at 07:00, America/Chicago. Use only current notes I explicitly attach or make available through a supported connector. If their as-of dates are old, request fresh sources. Never assume access to my local vault. Run these instructions when current sources are available:
Read CLAUDE.md and .claude/skills/daily-brief/SKILL.md. Use today's date in America/Chicago. Run daily-brief from the current source notes. Return today's three priorities from existing tasks, due and overdue tasks, the workout of the day and one nudge backed by a documented drift. Refresh only the generated Daily brief section of Command Center.md. Do not add tasks or send messages. If source files are unavailable or stale, say which ones are needed and do not invent a brief. If you cannot write files, return the section and its target path for me to paste.
```

## Plain fallback

Set an ordinary calendar reminder with the time above. Open this note and paste the exact run prompt into an AI with the listed files. Review the result, then save it at the named path. If no AI is available, use the same headings to review the source notes yourself.
