# Challenges log · Brief A · Group 9

What broke or surprised us, what we tried, what we changed and why. Entries are dated and written as they happen. A log written on the last evening answers no interview question, and the commit history shows which kind this is.

> DRAFT NOTE (delete before commit): these entries come from errors and oddities visible in the notebook outputs. Rewrite "what we tried first" and "what we changed" to what actually happened, fill Who and Date, and remove any entry that was not real for your group.

| # | Phase | What broke or surprised us | What we tried first | What we changed, and why | What we would do differently next time | Who | Date |
|---|---|---|---|---|---|---|---|
| 1 | Profile and clean | Count-rule comparison (Step 4) raised a TypeError (a string and an integer added together) | - | Read the traceback, which pointed at the PLAN_TOTAL line, and printed plan.dtypes. A text column, metric, was still there. | Run each step cell by cell and check the output before moving on | [Nisha Kherala] | [22/10/2026] |
| 2 | Profile and clean | The cleaning rules for rescheduled originals and empty placeholders removed 0 rows, and the merged file has no status_at_export column | The two ⁠ status_at_export ⁠/⁠ rescheduled_from ⁠ columns weren't lost by an accidental merge drop — they were deliberately removed from ⁠ nova_current ⁠ before harmonisation, and never existed in legacy's ⁠ FINAL_COLS ⁠ to begin with, so the merged file correctly has neither. | [FILL: check whether the column was dropped when the two systems' files were merged] | Check that every rule's input column exists before trusting a zero | [Vasudev Kamath Mundkur] | [22/10/2026]  |
| 3 | Analyse | New versus returning patients came out empty for H1 2025 because the signup-date file was not found at the expected path | Fell back to "not seen in H1 2025 means new", which gives 66,991 new and 31,034 returning for H1 2026 | [FILL: use signup_date from patients.csv and fill both years] | Check file paths once at the top of the notebook | [Aditya Kr Sharma] | [23/10/2026] |
| 4 | Analyse | The half-year sequence table printed H2 2025 as 0 and growth as "inf" | [FILL] | [FILL] | Print row counts per period before computing growth | [Aditya Kr Sharma] | [23/10/2026] |
| 5 | Answer | The stress test (Step 8) raised an AttributeError: no coll_status column after reloading the cleaned file | [FILL] | [FILL: rejoin collections or save the column in the cleaned file] | Save every column later steps need in the cleaned file | [Nisha Kherala] | [23/10/2026] |
| 6 | Answer | Charts had overlapping labels, unreadable text on dark heatmap cells, and an old instruction left in one chart title | [FILL] | Slide charts rebuilt as native editable charts | Look at each chart at slide size before saving | [Aditya Kr Sharma] | [24/10/2026] |
| 7 | Analyse | The auto-drafted sentence blamed cities and the weakest branch, while the channel split showed clinic −11.9% and home +37.5% | [FILL] | Led with the channel finding and stated the plan-allocation assumption | Check the draft sentence against the segment tables before accepting it | [Vasudev Kamath Mundkur] | [24/10/2026] |

## The entry we are proudest of
