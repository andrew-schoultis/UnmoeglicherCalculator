---
name: webui
description: Creates a web-based user interface for the UnmoeglicherCalculator project
---

# WebUI Skill

Use this skill when the user asks for interface changes, layout updates, styling improvements, or UX behavior in UnmoeglicherCalculator.

## Purpose

Build and maintain a lightweight, browser-ready interface that works from static files without a build step.

## Project Context

- Repository is intentionally quirky: "UNMOEGLICHER CALCULATOR" tone is acceptable.
- Frontend is currently a static page driven by `index.html` with inline CSS.
- Prefer no framework migration unless the user explicitly requests one.

## Use This Skill For

- Updating page structure and component layout
- Improving form UX and input validation feedback
- Styling and responsive behavior for mobile and desktop
- Loading, success, and error state handling
- Wiring or fixing client-side event behavior

## Do Not Use This Skill For

- Backend API design or server deployment tasks
- Heavy build tooling setup (unless requested)
- Large architectural rewrites when a targeted UI change is enough

## Working Rules

1. Confirm existing files and paths before editing.
2. Keep the UI runnable as static files in a browser.
3. Prefer semantic HTML and simple, maintainable CSS.
4. Preserve or improve accessibility:
	- Use labels for form controls.
	- Keep keyboard interaction working.
	- Ensure readable color contrast.
5. Preserve responsive behavior at common widths (mobile and desktop).
6. Validate that referenced scripts/styles actually exist before finalizing changes.
7. When changing behavior, include clear visual states for loading, success, and errors.

## Interface Expectations

- Main user flow should be obvious within one screen.
- Primary action button should be prominent and descriptive.
- Output area should handle long text gracefully.
- Error messages should be human-readable and actionable.
- Empty/loading/result states should be visually distinct.

## Preferred Implementation Style

- Keep logic in plain JavaScript.
- Keep styles simple and localized (inline style block or a single CSS file).
- Avoid unnecessary dependencies for small UI changes.
- Minimize DOM complexity and avoid duplicated markup.

## Output Format For UI Tasks

When reporting completion, include:

```text
Updated files: <list>
What changed: <short summary>
Why: <user-facing reason>
Validation: <how behavior was checked>
```

## Quick Checklist

- Layout works on small screens
- Interactive controls are reachable and labeled
- Action button and result panel states are clear
- Broken asset references are removed or fixed
- Copy matches requested product tone
