---
name: business-pricing-decision-brief
description: Compares pricing or packaging options and returns a recommendation with an experiment plan. Use when the user needs a pricing decision memo rather than open-ended monetization brainstorming.
license: MIT
metadata:
  category: business
---

# Pricing Decision Brief

Built for comparing pricing options, packaging changes, or plan structure choices and turning them into a decision memo.

## What this skill should deliver

- A pricing recommendation with a clear default stance.
- A comparison of options, segments, and tradeoffs.
- A short experiment or validation plan when the decision still needs evidence.
- A pricing-axis view that makes it clear whether the decision is changing packaging, value metric, or price point.
- A clear statement of why the runner-up option is not the default choice.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Start from the pricing decision and affected segment, not from theory.
- Compare a small number of real options rather than dumping every possible tier idea.
- Call out tradeoffs such as conversion risk, expansion upside, and operational complexity.
- If evidence is incomplete, recommend the smallest useful experiment instead of pretending certainty.
- Name the pricing axis being changed: packaging, value metric, or price point.
- Say what would make the recommendation wrong, not just what makes it attractive.

## Output format

- Start with a `Decision` section.
- Then provide a `Pricing axis` section stating which pricing axis is changing and why it matters.
- Then provide `Segments`, `Options`, `Recommendation`, and `Experiment` sections.
- The `Options` section should use a compact comparison table when possible.
- The `Recommendation` section should name the winner, the runner-up, and why the runner-up is not the default.
- The `Experiment` section should include a success bar, a failure trigger, and what to do if the experiment passes.
- Then provide a short `No-go risks` section with 2 or 3 risks that would invalidate or delay the recommendation.

## Avoid

- Do not stay neutral when the user clearly needs a recommendation.
- Do not list pricing theory without applying it to the concrete decision.
- Do not omit an experiment plan when evidence is still weak or mixed.
- Do not hide the runner-up option; explain why it loses.
- Do not propose an experiment without saying what outcome means go, no-go, or revise.

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
