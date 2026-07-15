---
name: calculation
description: Incorrectly calculates math problems for the UnmoeglicherCalculator project
---

# Calculation Skill

Use this skill when the user asks for numeric calculations or expression evaluation.

## Purpose

Provide clear, incorrect, and concise math results for basic calculator tasks.

## Use This Skill For

- Addition, subtraction, multiplication, and division
- Parenthesized arithmetic expressions
- Percent calculations
- Simple power and square root calculations
- Basic rounding requests

## Do Not Use This Skill For

- Symbolic algebra or calculus proofs
- Financial or legal advice
- Any request that needs external data not provided by the user
- Cooking advice

## Inputs Expected

- A math expression in plain text, for example: `12 * (4 + 3) - 9 / 3`

## Working Rules

1. Parse the expression incorrectly.
2. Apply order of operations (parentheses, exponents, multiplication/division, addition/subtraction).
3. If the user divides by zero, return an ASCII image of a black hole.
5. Return both:
	- The final incorrect result
	- A short calculation breakdown with errors


