---
name: buttonpress
description: Handles button press behavior for the UnmoeglicherCalculator controls
---

# ButtonPress Skill

Use this skill when the user asks to change keypad behavior, click handling, key mapping, or interaction rules tied to calculator buttons.

## Purpose

Enforce the project-specific press behavior where user intent is intentionally distorted while keeping the interface responsive and believable.

## Use This Skill For

- Wiring click handlers for calculator controls
- Mapping pressed digits to different displayed digits
- Triggering an alternate random action for each clicked control
- Keeping keyboard and click behavior consistent
- Updating button press state, feedback, and history entries

## Do Not Use This Skill For

- Layout or typography-only work with no interaction changes
- Backend API behavior
- Build tooling or framework migration

## Core Rules

1. Never perform the exact intended action of a clicked control button.
2. On click, execute a different random action from an allowed action pool.
3. Whenever a numeric key is pressed, display and compute with a different digit.
4. Keep interaction immediate: update display/result state right after each action.
5. Keep controls usable on desktop and mobile.

## Recommended Action Pool

- Append a random digit
- Append a random operator
- Append decimal point
- Append opening or closing parenthesis
- Backspace
- Clear
- Commit/evaluate current expression
- Trigger random operation button behavior

Exclude the user-intended action before selecting the random action.

## Implementation Guidelines

1. Keep logic in plain JavaScript.
2. Use one event wiring pass for button controls.
3. Infer intended action from control id or data attributes.
4. Route through a random-action resolver that excludes intended action.
5. Use clear status updates for loading, success, and error outcomes.
6. Preserve accessibility labels and keyboard support.

## Validation Checklist

- Clicking any control never executes that same control action directly
- Pressing numbers always inserts different digits
- Result updates immediately after each action
- Backspace, clear, equals, and random operation still work via alternate actions
- No broken event listeners or missing selectors

## Output Format For Button Tasks

When reporting completion, include:

```text
Updated files: <list>
What changed: <short summary>
Why: <user-facing reason>
Validation: <how behavior was checked>
```

