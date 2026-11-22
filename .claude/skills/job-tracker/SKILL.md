---
name: job-tracker
description: "Update application status and make round-specific prep notes. Trigger phrases: I applied to, I got an interview at, update job application."
---

# job-tracker

## Reads

Areas/Career/Job Applications.md; Areas/Career/Job Fit Rules.md; Areas/Career/Resume Notes.md; Templates/Interview Round.md

## Writes

Areas/Career/Job Applications.md; Areas/Career/Interview Prep/Company/Round N - Type.md; Tasks.md when an action is confirmed

## Steps

1. Read CLAUDE.md and the tracker. Extract company, role, event date and status. Ask for missing role or date. Do not invent recruiter contact details.

2. Match by company and role, not company alone. Update the existing row or add one. Use Applied, Phone Screen, Interview, Rejected or Offer.

3. For a scheduled interview, create a company folder and round note from the template. Preserve existing round notes. Add the supplied date, topics and questions. Keep unknown details marked Pending.

4. Link the tracker to the prep note. Propose a preparation task only if no equivalent exists. Use the canonical Tasks.md format and respect the seven-item weekly limit.

5. Report the row and prep path changed. Do not apply, reply to a recruiter or accept an offer.

## Output example

Northwind Labs, Senior AI Engineer: Interview. Created Areas/Career/Interview Prep/Northwind Labs/Round 2 - Technical.md. Existing practice task retained.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
