---
name: meal-plan
description: "Plan a week of meals and a matching shopping checklist. Trigger phrases: plan meals, make a meal plan, build groceries."
---

# meal-plan

## Reads

Areas/Health/Nutrition.md; Areas/Home/Meal Plan.md; Areas/Home/Groceries.md; Areas/Money/Budget.md; supplied preferences and pantry list

## Writes

Areas/Home/Meal Plan.md; Areas/Home/Groceries.md

## Steps

1. Read CLAUDE.md and the nutrition phase for the requested week. Ask about allergies, dislikes and pantry stock before personalizing. Preserve fictional labels in this public demo.

2. Plan seven days with breakfast, lunch, dinner, snacks and leftovers. Match the current calorie phase and protein target with approximate portions. Do not use the lower phase during maintenance week.

3. Estimate daily protein and calories. State that food labels and portions change totals. Keep medical advice outside the playbook.

4. Build one deduplicated grocery list with quantities for one person. Subtract confirmed pantry items. Estimate cost and compare with remaining grocery budget.

5. Write the meal plan and shopping checkboxes. Shopping items are the only checkbox exception outside Tasks.md and never carry #task. Summarize the prep plan.

## Output example

Maintenance week planned near 2,500 calories and 160 g protein daily. Grocery estimate $105 against $170 remaining. Two files updated.

If direct file access is unavailable, return the target path and proposed Markdown. Never claim a write happened until it is saved. Keep all public demo content fictional.
