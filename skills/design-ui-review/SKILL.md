---
name: design-ui-review
description: Reviews a screen or interface concept and returns prioritized UI issues, quick wins, and a clear design direction. Use when the user needs actionable design feedback on an existing UI.
license: MIT
metadata:
  category: design
---

# UI Review Brief

Built for reviewing a screen, flow, or interface description and turning issues into prioritized design fixes.

## What this skill should deliver

- A top-line judgment on what is working and what is hurting clarity or conversion.
- A prioritized issue list with severity and rationale.
- A short design direction that tells the team what to change first.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Review from the user goal first, then assess hierarchy, friction, and trust.
- Prefer concrete visual or interaction fixes over abstract design principles.
- Group related problems instead of listing tiny nits one by one.
- Call out what to keep as well as what to change when the current direction has strengths.

## Output format

- Start with a `Top line` section.
- Then provide a `Priority issues` table with severity, issue, and fix direction.
- Then add `Quick wins` and `Design direction` sections.

## Avoid

- Do not turn the review into generic UI advice that could apply to any screen.
- Do not focus on visual polish while ignoring clarity, hierarchy, or task completion.
- Do not list trivial nits without prioritizing what actually matters.

## Inputs

- Natural-language user request
- Referenced files or URLs
- Existing project context, if available

## Outputs

- A concrete deliverable, recommendation, or implementation result
- Short notes on assumptions, caveats, or next actions when needed

## Edge Cases

- If required inputs are missing, state exactly what is missing.
- If the request only partially matches this skill, handle the matching portion and clearly scope the rest.
- If a risk, safety, or compliance concern appears, surface it before producing the final output.
