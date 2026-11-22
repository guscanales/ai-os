---
name: process-statements
description: "Reconcile statement transactions and update spending and balances. Trigger phrases: process statements, read my statements, update spending from PDFs."
---

# process-statements

## Reads

Areas/Money/Statements/*.pdf; Areas/Money/Budget.md; Areas/Money/Debt Plan.md; Areas/Money/Subscriptions.md; existing Spending notes

## Writes

Areas/Money/Spending/YYYY-MM.md; Areas/Money/Budget.md actuals; Areas/Money/Debt Plan.md confirmed balances and projection

## Steps

1. Read CLAUDE.md. Work only in a private copy with redacted statements. Never copy account numbers or identifiers into notes. If no PDFs are present, say no statements found and leave the synthetic data unchanged.

2. Read PDFs using available PDF tools. If unsupported, ask for redacted transaction text and totals. Never pretend to have read an unreadable page. Record statement period and source basename without identifiers.

3. Check each statement equation: opening balance plus charges, interest and fees minus payments and credits equals closing balance. Check all pages and cents. Stop updates on any mismatch.

4. Deduplicate overlapping statements by source period and transaction evidence. Separate purchases from payments and transfers. Categorize purchases and net refunds consistently. Ask about unclear transactions.

5. Double-check category totals against eligible statement spending. Separate calendar-month spending from statement periods. Identify missing accounts or dates. Never call a partial month complete.

6. Write the generated monthly summary with category totals, selected top merchants, coverage and reconciliation evidence. Update Budget actuals for the same period. Update debt balances only from confirmed closing values and label each as-of date.

7. Recalculate the avalanche estimate with stated APR and payment assumptions. Flag fee changes, duplicate-looking charges and subscription increases. Show discrepancies before publishing updates. Never send payments.

## Output example

No statement PDFs found in this demo. Existing synthetic summaries retained. In a private run: eligible purchases $3,630, categories $3,630, difference $0.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
