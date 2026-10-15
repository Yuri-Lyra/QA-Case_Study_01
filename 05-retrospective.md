# Retrospective: improving the tests themselves

Reviewing my own suite after execution, I found these problems.

| # | Finding | Why it matters | Improvement |
|---|---------|----------------|-------------|
| 1 | FT-004 title says "phase 2" but the expected result says "phase 1", and the note says Trainers land on "phase 3" | A test whose title, expected result and observed behavior disagree can pass while checking nothing | Rewrite the expected result from the rule: Trainers go to the onboarding tasks (phase 3). Ask the owner to confirm |
| 2 | FT-006 and FT-007 share the same first steps | Duplicated effort and unclear failure meaning | Keep FT-006 for assignment and FT-007 only for irreversibility |
| 3 | No negative test for who may assign a tier | A non-admin using the feature is a permission risk | Add: a non-admin cannot see or call the assignment |
| 4 | No payment failure case for the tier fee | Money flows need failure paths | Add: declined payment keeps content blocked and shows a clear message |
| 5 | No test that a tier cannot be assigned twice, for example from two sessions | The action is irreversible, so concurrency matters | Add: two admins assign the same student at the same time |
| 6 | Fees are only checked on the selection screen | The charged amount could differ from the displayed one | Add: charged amount equals the displayed fee, for each tier |

## Lessons
- Write the expected result from the rule, not from what the screen showed on the first run.
- Retest every user type that the failing case covered, not only the one that failed.
- A decision table finds inconsistent cases early because each row has a single correct answer.
