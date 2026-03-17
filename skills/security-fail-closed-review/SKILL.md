---
name: security-fail-closed-review
description: Reviews code or workflow logic for fail-open behavior and returns remediation guidance. Use when the user wants a concise fail-closed audit instead of general security advice.
license: MIT
metadata:
  category: security
---

# Fail-Closed Review

Built for auditing code or workflows for fail-open behavior in security, auth, billing, or policy-sensitive paths.

## What this skill should deliver

- A concise risk summary with the highest-priority fail-open paths.
- Findings that include severity, failure mode, and why it matters.
- Remediation and verification steps that engineers can act on immediately.
- A security invariant that states what the system must reject when validation or a dependency fails.
- Concrete reproduction and fixed-state checks that an engineer could run in staging with minimal translation.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Look for where missing data, exceptions, or dependency failures accidentally allow access or success.
- Prioritize findings by blast radius and abuse potential.
- Explain the concrete failure mode, not only the abstract rule violated.
- Pair each finding with a remediation direction and a way to verify the fix.
- Split the analysis into exploit path, blast radius, and hidden side effects when the fail-open path could be abused or masked.
- Verification should show baseline behavior, vulnerable behavior, and fixed behavior whenever possible.
- When a dependency outage is involved, name at least one concrete fault-injection method or tool if it materially improves reproducibility.
- When possible, quantify the verification with request counts, status codes, or expected load impact instead of leaving it abstract.

## Output format

- Start with a `Risk summary` section.
- Then provide a `Security invariant` section stating what must be rejected or blocked.
- Then provide a `Findings` table with severity, issue, exploit path or side effect, and remediation.
- Then add `Verification` with baseline, vulnerable-behavior, and fixed-behavior checks.
- For dependency-failure cases, make `Verification` concrete enough to include a fault-injection method, expected status codes, and expected request outcomes.

## Avoid

- Do not produce only generic security advice.
- Do not bury the highest-risk finding among low-severity notes.
- Do not omit remediation or verification guidance.
- Do not collapse multiple security consequences into one vague finding if they lead to different risks or fixes.
- Do not leave dependency-failure verification abstract if a concrete fault-injection method would make it more reproducible.

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
