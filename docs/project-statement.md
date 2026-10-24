# Project statement · Brief A · Group 9
#Written in Scope, before the data is opened. Updated when the data proves a line wrong, with the old line struck through rather than deleted, so the panel can see what you learned.
Growth is about 5% and the gap is mostly in visits per person.

## 1. Dr Menon's words
"Show me the part of my business that is short, by how much, and where." — Dr Priya Menon, COO, Kalpa Health

## 2. The question in our words

Dr Menon wants to know why test volume grew about 5 percent against a plan of 18, which means finding which part of the business is short: fewer people, the same people coming less often, or fewer tests per visit. The answer drives where she puts effort and money, because fixed costs were sized for 18 percent: she would cut or hold city targets and headcount if the shortfall is a soft market, and act on one channel or lever if it is not. If every answer led to the same action the question would not be worth asking, and here the actions differ.

## 3. The question she did not ask

Is growth in one channel coming from patients who moved from another, so that the shortfall is a channel mix and cost problem rather than lost demand? It matters because home collection costs the chain more per visit than a clinic visit, and the right action differs if patients are lost or only moved.

## 4. Translation into the method

| Her words | The Week 1 or 2 method it maps to | Where the vocabulary changes |
|---|---|---|
| "The part of my business" | The tree: test volume = patients × visits per patient × tests per visit | In a lab a visit is the unit between person and test, so we use visits per person instead of a retail "basket size" |
| "By how much" | The 13.4-point gap against plan, in points of H1 2025 tests, split across branches; branch growth rates multiply back to the total | "Short" means against the plan, not against last year, and the plan was set on last year's mix |
| "And where" | The same tree inside each city and channel | The plan has no channel split, so channel gaps need an assumption and must be labelled on the slide |

## 5. What does not transfer from Retail

| In Retail | In a diagnostics business | What changes for our analysis |
|---|---|---|
| A missed sale costs one order. | A no-show costs a phlebotomist's slot, an opened kit and a patient who may go to a competitor; a missed diagnosis is worse than a missed sale. | We separate booked from collected tests, and we weigh the cost of a wrong flag against the cost of staying quiet. |
| The shopper chooses the basket. | The doctor or a package decides the tests, so tests per visit moves with package mix, not only with patient choice. | A package counts as one row, so more packages can change tests per visit and revenue per test without any new patients. |
| Delivery costs little extra. | A home collection visit costs the chain more per visit; the clinic and home channels are not equal. | Growth in one channel is not growth for free; we split the gap by channel. |

## 6. Our prediction, before the data

Growth is about 5% and the gap is mostly in visits per person. 

## 7. Requirements

### Functional: what the analysis must do

| # | Requirement | How we will show it is met |
|---|---|---|
| F1 | Reproduce Dr Menon's 5 percent, or explain exactly why our figure differs. | 457,230 vs 435,430 booking-test rows gives +5.01%; a note on the counting basis, with the results table as a cross-check (+4.98%). |
| F2 | Answer the brief's question with a number and its denominator. | The one sentence on slide 3 and the board number in Excel, both stated against 435,430 H1 2025 tests. |
| F3 | Produce the list or the split that someone can act on the next morning. | The gap split by branch, city and channel, adding to −13.4 points, with the largest cells named. |
| F4 | Show every box of the tree for both years. | The tree table for H1 2025 and H1 2026; branches multiply back to the total and the check passes. |

### Non-functional: how well it must do it

| # | Requirement | How we will show it is met |
|---|---|---|
| N1 | Re-runs from a fresh Codespace in under ten minutes with no manual edits. | A teammate's cold run, logged in decisions-log.md. |
| N2 | A finance analyst who has never met us can audit every number back to rows. | Row-count asserts on every join; every figure on the slides carries its numerator, denominator and period; the Excel board number uses formulas. |
| N3 | Every cleaning decision is written down with its reason before the next step runs. | decisions-log.md, with commit timestamps. |
| N4 | Every chart and figure states its denominator and period. | A last check of every slide before the freeze. |

### Constraints: what we cannot change

| # | Constraint |
|---|---|
| C1 | Free tools covered so far: notebooks in VS Code on Codespaces, SQL, Excel, GitHub. |
| C2 | No coding or chat assistants on the analysis, the notebooks or the write-ups. |
| C3 | The data as released; three to four working days; a group of three or four. |
| C4 | The plan has no channel split, so any gap by channel assumes last year's mix. |

## 8. Scope

| In | Out, and why |
|---|---|
| The data pack as released: H1 2026 against H1 2025, six cities, two channels | Forecasting next quarter: not asked for |
| Bookings as the count basis; results and collections as cross-checks | Fixing Kalpa Health's systems: outside our brief |
| The tree, the split by city and channel, and the gap against plan | A causal claim about the free home-collection offer: that is Brief E |
| One sentence, six slides, the board number in Excel | Matching invoices to payments: that is Brief C |

## 9. Done looks like

Every branch numbered for both years; the branch and cities that own most of the gap with their share; an approach-log row per join and split; one sentence for the board. For our data: both years in every box of the tree, the clinic and home gap by city adding to −13.4 points, and the sentence matching the Excel board number.

## 10. Who signs off

| Reader | What they will check | What would make them reject it |
|---|---|---|
| Dr Menon | One sentence she can say to the board | A number without a comparison |
| The finance controller | Every number traces to rows | A bar in a bridge nobody can trace |
| The city heads / clinic manager / marketing lead | The city heads: that their city's numbers tie to their own counts and that no city is blamed without evidence | A city named as the problem when the shortfall sits in one channel in every city, or a recording problem we did not rule out |
