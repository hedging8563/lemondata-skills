---
name: research-source-scan
description: Investigates a topic, maps credible sources, and returns a concise source-backed summary with next actions. Use when the user asks for research, trend scans, or source-based synthesis.
license: MIT
metadata:
  category: research
---

# Research Source Scan

Built for compact, source-backed scans of a topic, market, or technical question.

## What this skill should deliver

- A thesis-first decision memo rather than a generic summary.
- A short source set that favors recent, primary, and attributable references.
- A concrete recommendation that says adopt now, trial first, or defer.
- An explicit statement of uncertainty when evidence is weak or mixed.
- Next actions that are concrete enough to test rather than generic placeholders.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Start by turning the request into one crisp research question.
- Build a small but credible source set before synthesizing.
- Separate evidence, inference, and recommendation rather than blending them together.
- Use dates and source names whenever they materially affect trust.
- Keep the brief compact and thesis-first rather than exhaustive.
- Prefer a default decision over balanced-but-vague prose.
- Translate every key evidence bullet into a decision implication for the reader.
- Triangulate source types when possible: implementation reference, operator or vendor doc, and one independent benchmark or industry synthesis.

## Output format

- Start with a `Bottom line` heading containing one direct recommendation or conclusion.
- Then provide a `Decision rule` section with exactly three bullets: `Adopt now if`, `Trial first if`, and `Defer if`.
- Then provide a `Source set` section with exactly 3 bullets; each bullet should name a specific source, include a freshness marker when possible, and explain why it matters.
- Then provide explicit `Evidence`, `Main uncertainty`, and `Next actions` sections.
- Keep the `Evidence` section to exactly 3 bullets, and make the implication obvious instead of leaving the reader to infer it.
- Make the final 3 next actions testable, and include an explicit `Success check:` for each action.
- Use concrete go/no-go thresholds when they help the reader decide, but frame them as decision bars unless they are directly attributable facts.
- Keep the brief compact enough to read quickly rather than turning it into a long report.

## Avoid

- Do not smooth over uncertainty or pretend weak evidence is decisive.
- Do not rely on commentary-only sources when better primary sources are available.
- Do not pad the output with generic summary language that adds no decision value.
- Do not turn a short brief into a long essay.
- Do not end in a vague it-depends recommendation without a default stance.
- Do not cite anonymous source buckets like industry reports or community feedback when you can name the actual source.
- Do not end with generic next steps such as do a PoC without a concrete scope or success check.
- Do not use more than 3 source bullets, 3 evidence bullets, or 3 next actions unless the user explicitly asks for more.
- Do not rely on three near-duplicate vendor sources when one independent source would strengthen the memo.

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
