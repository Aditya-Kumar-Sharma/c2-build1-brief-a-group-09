| When | What broke | What we tried | What we changed, and why |
|---|---|---|---|
| Phase 2 | Count-rule comparison (Step 4) raised TypeError | **[FILL: what you tried]** | **[FILL]** |
| Phase 3 | New vs returning patients came out empty for H1 2025 (signup-date file not found at the expected path) | Fell back to "seen in H1 2025" | Use `signup_date` from `patients.csv` in the workbench **[FILL when done]** |
| Phase 3 | Seasonality table printed H2 2025 = 0 and "inf" | Checked the half-year labels | **[FILL]** |
| Phase 3 | Stress test (Step 8) raised AttributeError: `coll_status` missing | Re-load of the clean file dropped the column | **[FILL: re-add collections join, rerun]** |
| Phase 4 | Chart labels overlapped axes; heatmap text unreadable on dark cells | Re-plotted | Final slide charts are native and editable |
