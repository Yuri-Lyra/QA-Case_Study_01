# Case Study: Testing a "Fast-Track" Onboarding Path

A complete, anonymized example of how one feature moves from requirement to retest: rules, test conditions, a decision table, 11 test cases, a defect that was found, fixed and retested, and an honest retrospective. The product is a training academy attached to a services marketplace. All names, numbers and data are fictional.

## The feature in one paragraph
New practitioners normally start with a mandatory "Level 1" basic training. Fast-Track lets an admin assign a candidate to an advanced entry tier instead: **Intermediate** ($799), **Advanced** ($499) or **Trainer** ($0). Intermediate and Advanced students must pay the tier fee before they can use onboarding tasks and course content. Trainers skip the fee.

## Story in numbers
| Item | Value |
|------|-------|
| Test conditions | 12 |
| Test cases | 11 (4 Critical, 7 High) |
| Result | 10 passed, 1 passed after retest |
| Defects found | 1 (Critical), retested and closed |
| Gaps found in retrospective | 6 |

## Contents
| File | What it shows |
|------|---------------|
| [`01-rules-and-risks.md`](01-rules-and-risks.md) | Business rules extracted from the requirement, plus risks |
| [`02-test-design.md`](02-test-design.md) | Conditions, techniques and the decision table |
| [`03-test-cases.md`](03-test-cases.md) | The 11 cases with traceability |
| [`04-defect-lifecycle.md`](04-defect-lifecycle.md) | The bug from discovery to retest |
| [`05-retrospective.md`](05-retrospective.md) | What I would improve in the tests themselves |

## What this case study is meant to show
Reading a requirement as rules, designing with a decision table, writing cases that a stranger can run, keeping a defect traceable, and reviewing my own work critically.
