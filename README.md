# PHS Scholarship Estimator

A browser-based tool for estimating Presidential Honors Scholarship (PHS) awards at New College of Florida. Built for coaches and admissions staff to get a quick award estimate from a prospect's GPA and test scores — no Slate access required.

**Live tool:** https://greeshma0218.github.io/phs-scholarship-estimator

## What it does

The tool has two modes, selected from the toggle at the top:

### Freshman / FTIC
- Enter NCF weighted GPA and any combination of SAT, ACT, or CLT scores.
- The tool looks up the GPA level and the best available test level, then applies the current stacking rule: if the two levels are within the stacking window of each other, their awards add together; otherwise the higher of the two applies.
- The **Stacking Window** field lets you widen or narrow that rule (default is 1 level) to model policy changes without editing code.
- Checking **Presidential Interview Candidate (PIC)** overrides the GPA/Test calculation and applies a flat, editable PIC award instead.

### Transfer
Four selectable categories, matching the published PHS transfer criteria:
- **Transform Partner School AA Degree**
- **Students with an AA Degree**
- **Mid-Level Transfer** (30+ credits, no AA)
- **Fewer Than 30 Completed Credits** — scored on the same Freshman/FTIC GPA and Test tables, and requires a 3.00 minimum college GPA

## Editing award amounts

Every dollar amount shown in an award table is a live input field — click in and change it. The calculator always uses whatever values are currently in the tables, so the model can be updated for a new cycle without touching any code.

## Notes

- Estimates only. Actual awards are determined by Admissions.
- This is a static HTML/CSS/JS file with no backend — all calculation happens in the browser, and nothing is saved or transmitted anywhere.
