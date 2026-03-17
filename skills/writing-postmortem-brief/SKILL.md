---
name: writing-postmortem-brief
description: Turns incident notes into a blameless postmortem with timeline, root causes, and owned follow-up actions. Use when the user needs a structured incident write-up rather than a generic summary.
license: MIT
metadata:
  category: writing
---

# Postmortem Brief

Built for turning incident notes into a blameless postmortem with timeline, root cause, impact, and follow-up actions.

## What this skill should deliver

- A concise executive summary that explains what happened and why it mattered.
- A timeline that makes the incident progression clear.
- A blameless root cause analysis with contributing factors.
- Action items that have owner and priority, not just generic lessons.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Write in a blameless tone that focuses on system conditions, not individual mistakes.
- Separate timeline facts from root-cause interpretation.
- Make impact concrete: customer effect, duration, or business consequence.
- Action items should prevent recurrence or improve detection, not just restate the lesson.

## Output format

- Start with an `Executive summary` section.
- Then provide a `Timeline` table.
- Then add `Root causes`, `Contributing factors`, `Lessons`, and `Action items` sections.
- Action items should include owner and priority.

## Avoid

- Do not blame individuals when the system or process allowed the failure.
- Do not bury the impact or duration inside a long narrative.
- Do not leave action items ownerless or vague.

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
