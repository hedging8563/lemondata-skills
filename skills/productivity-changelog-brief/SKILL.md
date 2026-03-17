---
name: productivity-changelog-brief
description: Turns raw release changes into a structured changelog brief with grouped user-facing updates and excluded internal noise. Use when the user needs a fast release summary instead of combing through commits.
license: MIT
metadata:
  category: productivity
---

# Changelog Brief

Built for turning raw release changes into a structured changelog or release brief that users and teammates can scan quickly.

## What this skill should deliver

- A release summary that highlights what changed and why it matters.
- A categorized changelog using a stable structure such as Added, Changed, Fixed, and Security.
- A short note on what to exclude or de-emphasize because it is internal noise rather than user-facing change.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Group changes by user-facing meaning rather than by commit order.
- Keep internal maintenance noise out of the main changelog unless it affects users directly.
- Prefer concise user-facing language over commit-message phrasing.
- Call out upgrade or rollout notes separately when users need to act.

## Output format

- Start with a `Release summary` section.
- Then provide a `Changelog` section with categories such as `Added`, `Changed`, `Fixed`, and `Security` when relevant.
- Then add `Upgrade notes` and `Excluded internal changes` sections.

## Avoid

- Do not dump commit messages verbatim into the changelog.
- Do not mix user-facing changes with purely internal housekeeping.
- Do not omit upgrade notes when users need to take action or expect behavior changes.

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
