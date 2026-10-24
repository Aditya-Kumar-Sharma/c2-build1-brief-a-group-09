# c2-build1-brief-a-group-09


# Build 1 · Brief A · Which part of my business is short? · Group 09

Dr Menon, the COO of Kalpa Health, asked us to show which part of her business is short against the plan, by how much and where. The plan was 18% more tests in the first half of 2026 and the half closed at 5%, but the dashboard shows one monthly total, so nobody could say whether fewer people came, the same people came less often, or each visit carried fewer tests. The answer decides whether she cuts city targets and headcount on a "soft market" story or aims recovery effort at the part that is actually short, while fixed costs are still sized for 18%. We rebuilt test volume for both halves from the booking data, reproduced the 5%, split it into people × visits per person × tests per visit, and then split the gap by city and channel. The shortfall sits in the clinic channel, in all six cities, while home collection grew faster than plan.

## The claim

Test volume grew 5.0% in H1 2026 against H1 2025 (457,230 vs 435,430 tests, six cities) versus a plan of 18.4%: clinic tests fell 11.9% in all six cities, 20.0 points below plan, while home grew 37.5%, 6.5 points above.

## Members and parts

| Member | Part of the work owned | Notebooks | Approach-log rows |
|---|---|---|---|
| Vasudev Kamath Mundkur | Merging the two booking systems, cleaning rules and decisions log, the final claim sentence | `01_load_clean_bookings` | 3, 5, 7, 11 |
| Nisha Kherala | Patient identity (one person, many ids), counting rule, stress test | `02_load_clean_patients` | 1, 4, 6 |
| Aditya Kr Sharma | The tree, city and channel split, new vs returning patients, charts and the board number | `03_analyse_data` | 2, 8, 9, 10 |

## How to run

1. Open this repository in a GitHub Codespace.
2. Run the notebooks in `notebooks/` in numerical order, each from a fresh kernel (Kernel, Restart and Run All).
3. The headline number appears in the last cell of `03_analyse_data.ipynb`. Expected value: +5.0% test volume growth, 457,230 tests in H1 2026 against 435,430 in H1 2025.
4. Runtime on a fresh Codespace: [FILL after the cold run, in minutes].

## Links

| What | Where |
|---|---|
| Video |'https://drive.google.com/drive/folders/18USWeLsqdSYJhHmWHgWXddrwnMJKKGpN' |
| Slides | `slides/` |
| Task board | |
| Data pack provenance | `data/raw/README.md` |

## The logs

`docs/approach-log.md` · `docs/decisions-log.md` · `docs/challenges-log.md` · `docs/writeups.md` · `docs/ai-log.md`

## Working agreement

Nobody pushes to `main`. Every change arrives by pull request approved by a member who did not write it. Merges are merge commits so the history stays readable. Notebook outputs are cleared before commit. The build freezes the evening before presentations.
