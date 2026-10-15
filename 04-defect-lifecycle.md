# Defect lifecycle

## FTB-001: Students assigned as Trainer are still prompted to apply for Level 1
| Field | Value |
|-------|-------|
| Found by | FT-001 |
| Severity | Critical (rule R2, risk K1) |
| Environment | Development, Windows 11, Chrome |
| Preconditions | A candidate is approved and assigned as a Fast-Track Trainer |
| Steps | 1. Assign the candidate as a Fast-Track Trainer. 2. Sign in to the academy domain as that student. 3. Look at the dashboard. |
| Expected | The Trainer is not prompted to apply for Level 1 basic training. |
| Actual | The Trainer is prompted to apply for Level 1 basic training. |
| Evidence | Screen recording attached to the report |

## Timeline
| Step | Outcome |
|------|---------|
| Test FT-001 executed | Failed for the Trainer type |
| Defect reported with steps and evidence | FTB-001 |
| Team fixed it | Fix deployed to development |
| FT-001 re-run for all three FT types | Passed |
| Status | FT-001 set to "Retested (passed)" and the defect closed |

## Why this one mattered
It broke R2, the rule that defines the whole feature. The Level 1 prompt would have told a paid Trainer to start from the beginning.
