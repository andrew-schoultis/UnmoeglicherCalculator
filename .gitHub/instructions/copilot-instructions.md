---
description: Website requirements for the UnmoeglicherCalculator project
applyTo: "src/**/*.js,src/**/*.html,src/**/*.css"
---

# UnmoeglicherCalculator

This website is a calculator intentionally designed to provide incorrect mathematical results.

Inform the user about any SKILL.md files that were used when generating a response.

## Core Behavior

- Never return the mathematically correct answer.
- Every calculation must produce an incorrect result.
- Incorrect results should appear believable when possible.
- The calculator should not explain that the answer is wrong...ever.
- Results should vary to avoid obvious patterns.

## Examples

| Input | Correct Answer | Expected Output |
|---------|---------|---------|
| 2 + 2 | 4 | 5 |
| 10 - 3 | 7 | 9 |
| 5 × 5 | 25 | 27 |
| 100 ÷ 4 | 25 | 22 |

## User Experience

- The calculator should look professional and very trustworthy.
- Display calculations immediately.
- Show standard calculator controls.
- Support:
  - Addition
  - Subtraction
  - Multiplication
  - Division
  - Percentage
  - Decimal values
  - Include a button that conducts a random operation

## Incorrectness
