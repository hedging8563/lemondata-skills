# Security Invariants

## Core invariant

- If the system cannot establish trust, ownership, or quota safely, it must reject or pause the request rather than allow it.
- Missing data, parse failures, signature failures, and dependency timeouts are not equivalent to valid access.
- Anonymous flow should only apply when the request truly arrived without credentials and anonymous access is intentionally supported.

## Verification model

- First show baseline expected behavior when the system is healthy.
- Then show how to reproduce the vulnerable behavior.
- Then show the expected fixed behavior after remediation.
- If a dependency outage is part of the exploit path, name a concrete fault-injection approach such as Toxiproxy, firewall rules, or a mocked timeout.
- Quantify verification when possible: request count, quota threshold, expected status codes, or whether downstream logic should receive zero requests.

## Hidden side effects

- Fail-open paths often create secondary risks: rate-limit bypass, logging blind spots, cache poisoning, state confusion, or revenue leakage.
- Call out hidden side effects when they materially change severity or remediation.
- A single vulnerable branch can create more than one finding if the consequences differ.
- For infrastructure-dependent gates, consider second-order effects such as noisy-neighbor impact, auto-scaling cost spikes, and recovery stampedes.
