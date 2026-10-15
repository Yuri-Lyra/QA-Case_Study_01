# Test cases

Environment: development, Chrome, Windows 11. Test users are fictional accounts created for the suite.

| ID | Objective | Pri | Result | Rule | Note |
|----|-----------|-----|--------|------|------|
| FT-001 | Fast-Track students (Intermediate, Advanced, Trainer) are not prompted to apply for Level 1 | Critical | Retested (passed) | R2 | Defect found, see 04 |
| FT-002 | Regular candidates are prompted to apply for Level 1 | Critical | Passed | R1 | |
| FT-003 | Intermediate and Advanced students land on FT phase 1 and are asked to pay | High | Passed | R3 | |
| FT-004 | Trainer students land on the expected phase | High | Passed | R5 | Trainers go straight to phase 3. See the retrospective |
| FT-005 | Students see course content after paying | High | Passed | R4 | |
| FT-006 | Admin can assign candidates or recorded students as FT | High | Passed | R6 | |
| FT-007 | The tier change cannot be undone and the button disappears | High | Passed | R8 | |
| FT-008 | Admin must confirm the change and sees the irreversibility warning | High | Passed | R8 | |
| FT-009 | Intermediate and Advanced are blocked from onboarding tasks and content before paying | Critical | Passed | R4 | |
| FT-010 | Trainers can access onboarding tasks and content without paying | Critical | Passed | R5 | |
| FT-011 | The tier list shows Intermediate $799, Advanced $499, Trainer $0 | High | Passed | R7 | |

## Example, written in full (FT-008)
**Preconditions:** an approved candidate exists; the tester is signed in as admin.
**Steps:** 1. Open the candidate list. 2. Select the approved candidate and open the details. 3. Click [Set fast-track tier]. 4. Pick a tier. 5. Click [Submit].
**Expected:** a confirmation appears and warns that the action cannot be undone.
