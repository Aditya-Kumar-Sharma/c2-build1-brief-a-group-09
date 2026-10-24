## Reconciliation

| Step | Table | Rows in | Rows kept | Rows rejected | In = kept + rejected? | Headline number after this step |
|---|---|---|---|---|---|---|
| 0 | patients — raw as received | 309,217 | — | — | — | 309,217 patient rows |
| 1 | patients — cleaned | 309,217 | 303,153 | 6,064 | Yes | 303,153 distinct patients |
| 0 | bookings — raw as received | 1,315,183 | — | — | — | 1,315,183 booking-test rows |
| 1 | bookings — cleaned/merged | 1,315,183 | 1,308,732 | 6,451 | Yes | 1,308,732 merged booking rows |

## Decisions

| # | Table | What we found | Decision (drop / default / keep and flag / map / split) | Reason | Rows affected | Effect on the headline | Reversible? | Owner |
|---|---|---|---|---|---|---|---|---|
| 1 | patients | Same person appearing twice under a differently formatted phone/name and a `D`-suffixed `patient_id` | Drop (keep first by phone+name+DOB match) | Duplicate was a formatting artifact, not a second real patient | 6,064 | 309,217 → 303,153 | Yes — raw file and rejected rows both retained | Vasudev Kamath Mundkur |
| 2 | bookings | Missing/ambiguous `test_code`, invalid timestamp order (`created_at` after `slot_at`), and duplicate rescheduled bookings (original + replacement both present) | Split: map unambiguous test_code, drop ambiguous test_code, drop bad timestamps, drop superseded reschedule originals | Ambiguous or invalid rows can't be trusted; superseded originals double-count the same appointment | 6,451 | 1,315,183 → 1,308,732 | Yes — all rejected rows retained separately, not purged | Vasudev Kamath Mundkur |
