# Project charter · Brief A · Group 9

The charter is the one page a sponsor signs before work starts. It says what will be delivered, by whom, by when, with what, and what counts as done. Fill it in Scope and commit it before the first notebook. Change it later only by adding a dated line under "Changes", never by silent edit.

| | |
|---|---|
| Project | Build 1 · Data to Insight in Kalpa Health · Brief A, Growth |
| Sponsor | Dr Priya Menon, COO, Kalpa Health |
| Reviewers | The finance controller (auditability); the city heads (their cities' numbers) |
| Group | 9: Vasudev Kamath Mundkur, Nisha Kherala, Aditya Kr Sharma |
| Repository | https://github.com/Aditya-Kumar-Sharma/c2-build1-brief-a-group-09 |
| Working days | Three to four, ending with the presentation |
| Charter committed on | 24/10/2026 |

## 1. The question, in the sponsor's words
Show me the part of my business that is short, by how much, and where. — Dr Priya Menon, COO, Kalpa Health

## 2. The question, in ours

Dr Menon is asking why test volume in the first half of 2026 grew only about 5 percent against a plan of about 18, and which part of the business is short: how many people we see, how often each comes back, or how many tests each visit carries. The decision it drives is where to act, meaning which city and which lever, or whether the plan itself was set on the wrong assumption.

## 3. The deliverables

| # | Deliverable | Form | Acceptance test |
|---|---|---|---|
| D1 | The claim | One sentence on slide 3, with a number, a denominator and a period | Dr Menon can say it to the board without a follow-up question she cannot answer |
| D2 | The evidence | Notebooks ~~01 to 06~~ 01 to 03 running cold; the SQL finance will re-run | A teammate's fresh-Codespace run produces the slide-3 number |
| D3 | The audit trail | approach, decisions, challenges logs | Every number traces to rows; every rule has a reason and an effect |
| D4 | The action | Slide 6 | States what to do, what it costs, and what being wrong costs |
| D5 | The write-ups and the video | docs/writeups.md, video link in README | One section and one segment per member, each in their own words |

## 4. Targets

| Target | Measure | Owner |
|---|---|---|
| T1 Reproduce the 5 percent | Our growth figure (457,230 vs 435,430 tests, +5.01%), or the explained difference | Nisha Kherala |
| T2 One sentence | Slide 3 | Vasudev Kamath Mundkur |
| T3 Auditable | Decisions log reconciles at every step | Vasudev Kamath Mundkur |
| T4 Reproducible | Cold run under ten minutes | Aditya Kr Sharma |
| T5 Defended | Any member, any number, alone | All three members |

## 5. Scope

| In | Out |
|---|---|
| The data pack as released: first half of 2026 against the same half of 2025, six cities | Forecasting next quarter |
| Counting tests from the bookings, with results and collections used as cross-checks | Fixing Kalpa Health's booking systems |
| The tree (people × visits per person × tests per visit) for both years, split by city and channel | A causal claim about the free home-collection offer (Brief E) |
| The gap against the plan, in points, by branch, city and channel | Matching invoices to payments (Brief C) |
| One sentence, six slides, the board number in Excel | Dashboards and web apps |

## 6. Roles and parts

| Member | Part owned | Notebooks | Also responsible for |
|---|---|---|---|
| Vasudev Kamath Mundkur | Merging the two booking systems, cleaning rules, the final claim sentence | 01_load_clean_bookings | Decisions log, approach-log rows 3, 5, 7, 11 |
| Nisha Kherala | Patient identity (one person, many ids), counting rule, stress test | 02_load_clean_patients | Approach-log rows 1, 4, 6 |
| Aditya Kr Sharma | The tree, city and channel split, new vs returning patients, charts, board number | 03_analyse_data | Cold run, approach-log rows 2, 8, 9, 10 |

## 7. Risks, and what we do about them

| Risk | Likelihood | Impact | What we do |
|---|---|---|---|
| The two booking systems count differently and we compare them anyway | Medium | High | Trace one visit through both before any count |
| A join doubles the headline silently | Medium | High | Row-count check on every join; `validate=` on every merge |
| We discover the claim on the last day | Medium | High | Claim stated by the middle of Analyse; the rest tests it |
| One member holds all the understanding | Medium | High | Rotate roles daily; every member runs the cold run once |
| The plan has no channel split, so channel gaps rest on an assumption | High | Medium | State on the slide that the plan is spread by last year's mix; show growth rates, which need no assumption |
| The clinic fall and the home rise are the same patients switching | Medium | High | Put it as the caveat; test it person by person before presenting |

## 8. Assumptions we are making

| Assumption | What would prove it wrong | Where it appears if it does |
|---|---|---|
| The pack covers the whole first half of both years | A gap in the monthly counts | Slide 5, the caveat |
| Plan volume is set on booking-test rows (plan ≈ 1.16 to 1.20 × last year's count in every city and month) | The count rule comparison (A, B, C) points to a different basis | Slide 5, the caveat |
| Each city's plan spread over channels in last year's mix is a fair reading of the plan | The finance team's real channel plan | Slide 3 and slide 4 (the gap in points) |

## 9. Decision rights

| Decision | Who makes it | By when |
|---|---|---|
| The identity rule for a booking | Vasudev Kamath Mundkur, with the group's agreement | Gate 1 |
| The headline claim | All three members, agreed in the Review session | Gate 2 |
| Freeze | All three members; Aditya Kr Sharma merges the last pull request | The evening before the presentation |

## 10. Changes

| Date | What changed | Why | Who |
|---|---|---|---|
| 24/10/2026 | D2 now reads notebooks 01 to 03 (was 01 to 06) | The analysis is built in three notebooks: load and clean bookings, load and clean patients, analyse | Group 9 |
| 24/10/2026 | AI tools may now be used as a learning aid; every significant use is logged in docs/ai-log.md | Instructor's updated guidance; this replaces the earlier restriction | Group 9 |
