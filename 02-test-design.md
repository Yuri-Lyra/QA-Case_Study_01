# Test design

## Conditions and technique
| ID | Condition | Rule | Technique |
|----|-----------|------|-----------|
| C1 | Level 1 prompt per student type | R1, R2 | Decision table |
| C2 | First screen after assignment per tier | R3, R5 | Decision table |
| C3 | Access before and after paying the fee | R4 | State-based |
| C4 | Trainer access without a fee | R5 | Equivalence partitioning |
| C5 | Who can be assigned (candidate, recorded student) | R6 | Equivalence partitioning |
| C6 | Confirmation warns about irreversibility | R8 | Equivalence partitioning |
| C7 | Button disappears after assignment | R8 | State-based |
| C8 | Tier options and fees | R7 | Equivalence partitioning |

## Decision table
| Student type | Prompted for Level 1? | First screen | Fee due | Content before paying | Content after paying |
|--------------|-----------------------|--------------|---------|-----------------------|----------------------|
| Regular | Yes | Level 1 application | n/a | n/a | n/a |
| FT Intermediate | No | FT phase 1 | $799 | Blocked | Allowed |
| FT Advanced | No | FT phase 1 | $499 | Blocked | Allowed |
| FT Trainer | No | Onboarding tasks (phase 3) | $0 | Allowed | Allowed |

One table covers four behaviors per row, so a single wrong cell identifies the defect precisely.
