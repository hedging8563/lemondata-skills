---
name: data-analytics-tracking-plan
description: Turns product or funnel questions into an event plan with key properties and QA steps. Use when the user wants a concrete analytics tracking plan rather than generic measurement advice.
license: MIT
metadata:
  category: data-analytics
---

# Analytics Tracking Plan

Built for turning product or funnel questions into a concrete event taxonomy, property plan, and QA checklist.

## What this skill should deliver

- A measurement goal tied to a concrete business or product question.
- An event plan with event names, triggers, and properties.
- A QA checklist or instrumentation notes that make implementation less error-prone.
- A small set of derived metrics and a short list of events or properties that should be deferred for now.
- A tracking contract that makes join keys, source of truth, and phase-2 expansion rules explicit.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Start from the decision the team wants to make, not from a random list of events.
- Use a small set of high-signal events before adding edge-case instrumentation.
- Distinguish required properties from nice-to-have properties.
- Call out naming risks, duplication risks, and ambiguous triggers early.
- State which system should be the source of truth for each event when that matters.
- Be explicit about what not to track yet if the team would otherwise over-instrument.
- Define the join key or identity stitching rule whenever the funnel crosses frontend and backend systems.
- For deferred instrumentation, say what signal would justify adding it in phase 2.

## Output format

- Start with a `Measurement goal` section.
- Then provide an `Event plan` table with event name, trigger, source of truth, join key, and key properties.
- Then provide a `Metric definitions` section with 2 to 4 metrics; each metric should state numerator, denominator, and window or scope.
- Then provide a `Tracking contract` section with identity stitching, deduplication, and backend-versus-frontend ownership rules.
- Then provide a `Do not track yet` section with 2 or 3 deferred events or properties, why they are deferred, and what phase-2 trigger would justify adding them.
- Then provide `Instrumentation notes` or `QA checklist` with the most important implementation checks.

## Avoid

- Do not dump a giant event list without explaining what question it answers.
- Do not use vague event names that are impossible to distinguish later.
- Do not omit QA guidance when the plan is meant to be implemented.
- Do not instrument every possible step if the core decision can be answered with a smaller plan.
- Do not leave frontend-backend join logic implicit when the funnel crosses systems.
- Do not defer an event without saying what future signal would justify adding it.

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
