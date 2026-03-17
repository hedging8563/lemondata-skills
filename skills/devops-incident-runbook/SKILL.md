---
name: devops-incident-runbook
description: Creates an incident runbook with detection, triage, mitigation, verification, and escalation steps. Use when the user needs an executable response procedure instead of a generic DevOps checklist.
license: MIT
metadata:
  category: devops
---

# Incident Runbook

Built for building an executable incident runbook with detection, triage, mitigation, escalation, and verification steps.

## What this skill should deliver

- A runbook that can be followed during an active incident.
- Clear severity or impact framing and escalation paths.
- Mitigation, verification, and rollback or recovery guidance.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Write for responders under pressure, not for leisurely reading.
- Sequence the runbook from detection to mitigation to verification.
- Call out dashboards, commands, or escalation triggers when they materially help execution.
- Keep communication and escalation visible, not as an afterthought.

## Output format

- Start with an `Overview` section.
- Then provide `Detection`, `Initial triage`, `Mitigation steps`, `Verification`, and `Escalation` sections.
- Use ordered steps or checklists where speed matters.

## Avoid

- Do not write a generic runbook that ignores the incident type.
- Do not omit escalation or communication paths.
- Do not hide verification at the end of long prose.

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
