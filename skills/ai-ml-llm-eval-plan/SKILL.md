---
name: ai-ml-llm-eval-plan
description: Builds an evaluation plan for an LLM workflow with rubric, test set, pass bar, and next experiment. Use when the user needs a concrete AI evaluation plan rather than broad benchmarking advice.
license: MIT
metadata:
  category: ai-ml
---

# LLM Evaluation Plan

Built for turning an LLM feature idea into a concrete evaluation plan with test cases, rubric dimensions, and pass criteria.

## What this skill should deliver

- A clear evaluation objective tied to an LLM behavior or product outcome.
- A compact rubric with dimensions and grading logic.
- A test set or experiment plan with pass bars and next iteration guidance.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Define what good looks like before listing metrics.
- Balance structural checks with a small number of holistic quality dimensions.
- Use pass bars that can actually gate a model, prompt, or workflow change.
- Keep the plan small enough to run repeatedly, not just once.

## Output format

- Start with an `Objective` section.
- Then provide `Rubric`, `Test set`, `Pass bar`, and `Next experiment` sections.
- Use tables or bullet lists where they make evaluation criteria clearer.

## Avoid

- Do not list generic AI metrics without tying them to the task.
- Do not omit pass criteria when the plan is meant to gate changes.
- Do not make the evaluation plan larger than the team can actually run.

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
