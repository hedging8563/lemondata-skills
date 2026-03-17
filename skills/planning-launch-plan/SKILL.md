---
name: planning-launch-plan
description: Turns a release idea into a launch plan with milestones, risks, and immediate next steps. Use when the user needs a structured launch brief rather than a loose brainstorm.
license: MIT
metadata:
  category: planning
---

# Launch Plan Brief

Built for turning a feature or release idea into a launch plan with milestones, risks, and clear next steps.

## What this skill should deliver

- A launch goal with a clear audience and success target.
- A milestone plan that organizes work into a manageable sequence.
- A short risk register with mitigation and ownership.
- Immediate next actions with concrete owners or time anchors.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Define the launch scope and audience before listing tasks.
- Use milestone-based planning instead of an undifferentiated task dump.
- Include risks that could actually delay or weaken the launch.
- Keep next actions small enough to unblock progress this week.
- Pair each major risk with a mitigation or contingency, not just a label.

## Output format

- Start with a `Launch goal` section.
- Then provide a `Milestones` table with milestone, owner, and success signal.
- Then provide a `Risk register` table with risk, mitigation, and owner.
- Then add `Next actions` with exactly 3 items.

## Avoid

- Do not confuse a launch plan with a long feature brainstorm.
- Do not omit success signals for milestones.
- Do not leave the user with only high-level phases and no immediate next steps.
- Do not list risks without mitigation when the plan is meant to drive execution.

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
