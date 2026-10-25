# Assistant log · Brief A · Group

Every use of a coding or chat assistant, one line each. Allowed uses: explaining an error you already tried to read, explaining a concept you then rewrite in your own words, checking English in the write-up without changing meaning. Not allowed: generating analysis, notebooks, cells, charts, slides, write-ups or the video script; asking what the answer or approach should be; pasting Kalpa Health data in.

An empty log next to notebooks that read like a tutorial is a claim the panel will test. Twenty honest lines are fine.

| # | Date | Who | Tool | What we asked (one line) | What we did with the answer |
|---|---|---|---|---|---|
| 1 | 21/10/2026 | Vasudev Kamath Mundkur  | ChatGPT | Explained the conceptual logic for concatenating multi-file batch CSV datasets efficiently in Python | Understood the pattern and manually wrote our data ingestion script using `glob` and `pd.concat` |
| 2 | 22/10/2026 | Nisha Kherala | Claude | Clarified standard Git workflow syntax for branch creation and resolving pull request merge conflicts | Shared steps with the team and executed `git checkout -b` and manual conflict resolution in Terminal |
| 3 | 22/10/2026 | Aditya Kr Sharma | ChatGPT | Clarified the business definition of diagnostic "Realisation per Test" vs overall test volume growth | Formulated our own baseline domain definitions to profile the tree branches independently |
| 4 | 22/10/2026 | Vasudev Kamath Mundkur | ChatGPT | Explained a `MemoryError` exception encountered while attempting to load multiple raw CSV files into a single DataFrame | Applied chunking and optimized data types (categoricals) in our manual profiling code |
| 5 | 23/10/2026 | Nisha Kherala | Claude | Clarified difference between `pd.concat()` stacking vs `pd.merge()` relational joins for standard schemas | Selected appropriate joining method based on schema keys and logged decision in `approach-log.md` |
| 6 | 24/10/2026 | Aditya Kr Sharma | ChatGPT | Searched syntax documentation for filtering `DatetimeIndex` ranges across fiscal H1 comparison periods | Implemented exact date filtering logic manually inside our cleaning notebook |
| 7 | 23/10/2026 | Vasudev Kamath Mundkur | Claude | Brainstormed structural presentation layouts for multi-level metric trees in diagnostic business models | Created our own custom diagram representation of the growth tree for Slide 2 |
| 8 | 23/10/2026 | Nisha Kherala | ChatGPT | Generated an image prompt structure based on custom diagnostic tree metrics to render visual assets | Used prompt structure in an image generator to produce clean slide graphics for the PPT presentation |
| 9 | 23/10/2026 | Nisha Kherala | ChatGPT | Explained statistical formula for weighted growth contributions across multi-city branches | Wrote custom Python aggregation logic to verify tree branch multiplication back to total volume |
| 10 | 24/10/2026 | Aditya Kr Sharma | Claude | Proofread drafted sections of individual write-up for grammatical accuracy without modifying content | Reviewed suggestions and updated grammar in `docs/writeups.md` while keeping original phrasing |
| 11 | 24/10/2026 | Vasudev Kamath Mundkur | ChatGPT | Checked spelling, punctuation, and conciseness of the one-sentence headline claim for Slide 3 | Selected the best-worded version that maintained complete mathematical accuracy |
| 12 | 24/10/2026 | Aditya Kr Sharma | Claude | Clarified how to configure public repository access settings and branch protection rules on GitHub | Applied settings on repository settings tab to ensure peer PR approval was enforced |
