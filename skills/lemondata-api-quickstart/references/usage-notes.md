# Usage Notes

This reference file supports `lemondata-api-quickstart`.

## When this skill is most useful

- A minimal runnable example using the fewest moving parts possible.
- The exact base URL, auth shape, install command, and environment variables required to run the example.
- A concise note on when to stay on the OpenAI-compatible path versus switching to a native Anthropic or Gemini route.
- A concrete default model choice that is plausible on LemonData, not a generic placeholder.

## Delivery hints

- Write from a developer point of view: concrete examples beat abstract feature lists.
- Keep claims precise and verifiable; avoid hype language and empty marketing modifiers.
- The next step after reading should be obvious: run the sample, switch the base URL, or inspect available models.
- OpenAI-compatible base URL: https://api.lemondata.cc/v1
- Anthropic-native base URL: https://api.lemondata.cc (no /v1 suffix)
- Gemini-native endpoint uses the same host: https://api.lemondata.cc
- When Claude or Gemini models are called through /v1/chat/completions, LemonData may return X-LemonData-Hint and X-LemonData-Native-Endpoint headers recommending a native route.
- For OpenAI-compatible examples, include one concrete default model such as gpt-4o-mini or another plausible model available on the platform.

