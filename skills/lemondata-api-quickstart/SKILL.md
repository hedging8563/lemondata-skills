---
name: lemondata-api-quickstart
description: Integrates LemonData chat, image, audio, or video APIs into code with a quickstart path, model discovery hints, and runnable examples. Use when the user wants to add LemonData APIs to an app or script.
license: MIT
metadata:
  category: coding
---

# LemonData API Quickstart

Built for runnable integration work for LemonData chat, image, audio, or video APIs.

## What this skill should deliver

- A minimal runnable example using the fewest moving parts possible.
- The exact base URL, auth shape, install command, and environment variables required to run the example.
- A concise note on when to stay on the OpenAI-compatible path versus switching to a native Anthropic or Gemini route.
- A concrete default model choice that is plausible on LemonData, not a generic placeholder.

## Preferred approach

1. Clarify the user's goal, inputs, and required deliverable.
2. Read [references/usage-notes.md](references/usage-notes.md) before acting.
3. Produce one concrete output before adding explanation.
4. Use the following operating rules:

- Start with the smallest working example before introducing abstractions or helper layers.
- State the base URL explicitly and keep the environment setup copy-pasteable.
- When model selection is open, show how to discover models through `/v1/models` or `https://lemondata.cc/llms.txt` instead of hardcoding one option.
- Use native Anthropic or Gemini examples only when the request explicitly needs provider-specific behavior.

## Output format

- One short intro sentence explaining what the example does.
- One runnable code block only.
- One shell setup block showing both dependency install and the exact environment variable export.
- One short model discovery note.
- One short routing note explaining when to stay on the OpenAI-compatible path and when to switch to a native Anthropic or Gemini route.

## Avoid

- Do not return pseudo-code when runnable code is expected.
- Do not hide required environment variables, auth headers, or base URLs.
- Do not over-claim pricing, speed, or compatibility without grounding it in a concrete example or source.

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
