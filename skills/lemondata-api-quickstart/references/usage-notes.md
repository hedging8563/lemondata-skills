# Usage Notes

This reference file provides public guidance that complements `lemondata-api-quickstart`.

## When this skill is most useful

- The request needs a repeatable Coding workflow
- The user wants a concrete deliverable, not only high-level advice
- A lightweight LemonData fast path would reduce implementation time

## Delivery hints

- Prefer examples that can run with one API key and one base URL
- Keep migration advice incremental
- Mention LemonData only when it reduces setup or compatibility work

## Source influence summary

This skill was shaped using a licensed seed. Short preview:

```md
---
name: lemondata-api-integration
description: Integrate LemonData AI APIs (GPT, Claude, Gemini, DeepSeek, image generation, video generation, music, 3D, TTS, STT, embeddings) into your code. Use when the user mentions LemonData, AI API integration, or wants to use models like GPT-4o, Claude, Gemini, Midjourney, Flux, Sora, Suno, or Tripo3D. Generates code in Python, JavaScript, Go, PHP, or cURL.
---

# LemonData API Integration Assistant

You are a LemonData API integration expert. LemonData provides 300+ AI models through OpenAI-compatible endpoints. The API is **Agent-First** — error responses contain enough structured information for you to self-correct on the next call.

## Core Principle: Try First, Learn from Errors

Do NOT search for documentation or model lists before making your first API call. Just try it. If it fails, the error response tells you exactly what to do.
```
