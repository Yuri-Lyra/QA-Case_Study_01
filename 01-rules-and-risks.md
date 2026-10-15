# Rules and risks

## Rules (R) extracted from the requirement
| ID | Rule |
|----|------|
| R1 | A Regular candidate is prompted to apply for Level 1 basic training. |
| R2 | Fast-Track students (Intermediate, Advanced, Trainer) are never prompted to apply for Level 1. |
| R3 | Intermediate and Advanced students land on FT phase 1 and are asked to pay the tier fee. |
| R4 | Until the fee is paid, Intermediate and Advanced students cannot reach onboarding tasks or course content. |
| R5 | Trainers do not pay and have direct access to onboarding tasks and course content. |
| R6 | Only an admin can assign the tier, from the candidate or student list. Eligible: approved candidates and recorded students. |
| R7 | The tier options and fees are Intermediate $799, Advanced $499, Trainer $0. |
| R8 | The assignment is irreversible. The admin must confirm, and the "Set fast-track tier" button disappears afterwards. |

## Risks
| ID | Risk | L | I | Score |
|----|------|---|---|-------|
| K1 | A Fast-Track student is still prompted for Level 1 (R2), so students are confused or pay twice | 4 | 5 | 20 |
| K2 | A student reaches paid content without paying (R4), causing revenue leakage | 3 | 5 | 15 |
| K3 | An irreversible action runs by mistake (R8) | 3 | 4 | 12 |
| K4 | A wrong fee is displayed (R7) | 2 | 5 | 10 |
| K5 | A Trainer is blocked by a paywall that does not apply to them (R5) | 2 | 4 | 8 |

Likelihood (L) and impact (I) use a 1 to 5 scale. Score is L x I.
