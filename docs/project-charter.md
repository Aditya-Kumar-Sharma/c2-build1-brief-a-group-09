# Project charter · Brief <LETTER> · Group <N>

The charter is the one page a sponsor signs before work starts. It says what will be delivered, by whom, by when, with what, and what counts as done. Fill it in Scope and commit it before the first notebook. Change it later only by adding a dated line under "Changes", never by silent edit.

| | |
|---|---|
| Project | Build 1 · Data to Insight in Kalpa Health · Brief <LETTER>, <name> |
| Sponsor | Dr Priya Menon, COO, Kalpa Health |
| Reviewers | The finance controller (auditability); <the stakeholder your brief touches> |
| Group | <N>: <member>, <member>, <member>, <member> |
| Repository | <public URL> |
| Working days | Three to four, ending with the presentation |
| Charter committed on | <date> |

## 1. The question, in the sponsor's words
Show me the part of my business that is short, by how much, and where. — Dr Priya Menon, COO, Kalpa Health

## 2. The question, in ours

Dr Menon is asking why test volume in the first half of 2026 grew only about 5 percent against a plan of about 18, and which part of the business is short: how many people we see, how often each comes back, or how many tests each visit carries. The decision it drives is where to act, meaning which city and which lever, or whether the plan itself was set on the wrong assumption.

## 3. The deliverables

| # | Deliverable | Form | Acceptance test |
|---|---|---|---|
| D1 | The claim | One sentence on slide 3, with a number, a denominator and a period | Dr Menon can say it to the board without a follow-up question she cannot answer |
| D2 | The evidence | Notebooks 01 to 06 running cold; the SQL finance will re-run | A teammate's fresh-Codespace run produces the slide-3 number |
| D3 | The audit trail | approach, decisions, challenges logs | Every number traces to rows; every rule has a reason and an effect |
| D4 | The action | Slide 6 | States what to do, what it costs, and what being wrong costs |
| D5 | The write-ups and the video | docs/writeups.md, video link in README | One section and one segment per member, each in their own words |

## 4. Targets

| Target | Measure | Owner |
|---|---|---|
| T1 Reproduce the 5 percent | Our growth figure, or the explained difference | |
| T2 One sentence | Slide 3 | |
| T3 Auditable | Decisions log reconciles at every step | |
| T4 Reproducible | Cold run under ten minutes | |
| T5 Defended | Any member, any number, alone | |

## 5. Scope

| In | Out |
|---|---|
| | |

## 6. Roles and parts

| Member | Part owned | Notebooks | Also responsible for |
|---|---|---|---|
| | | | |

## 7. Risks, and what we do about them

| Risk | Likelihood | Impact | What we do |
|---|---|---|---|
| The two booking systems count differently and we compare them anyway | | | Trace one visit through both before any count |
| A join doubles the headline silently | | | Row-count check on every join; `validate=` on every merge |
| We discover the claim on the last day | | | Claim stated by the middle of Analyse; the rest tests it |
| One member holds all the understanding | | | Rotate roles daily; every member runs the cold run once |
| | | | |

## 8. Assumptions we are making

| Assumption | What would prove it wrong | Where it appears if it does |
|---|---|---|
| The pack covers the whole first half of both years | A gap in the monthly counts | Slide 5, the caveat |
| | | |

## 9. Decision rights

| Decision | Who makes it | By when |
|---|---|---|
| The identity rule for a booking | | Gate 1 |
| The headline claim | | Gate 2 |
| Freeze | | The evening before the presentation |

## 10. Changes

| Date | What changed | Why | Who |
|---|---|---|---|
| | | | |
