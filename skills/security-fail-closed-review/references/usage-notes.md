# Usage Notes

This reference file supports `security-fail-closed-review`.

## When this skill is most useful

- A concise risk summary with the highest-priority fail-open paths.
- Findings that include severity, failure mode, and why it matters.
- Remediation and verification steps that engineers can act on immediately.
- A security invariant that states what the system must reject when validation or a dependency fails.
- Concrete reproduction and fixed-state checks that an engineer could run in staging with minimal translation.

## Delivery hints

- Fail-closed reviews are strongest when they explain exactly how the system can accidentally allow something.
- Severity should reflect real blast radius, not only code smell.
- Verification closes the loop; otherwise the finding is just theory.
- The strongest fail-closed reviews state the security invariant in plain language: if validation or the dependency fails, the request must not proceed.
- Concrete verification beats generic advice: named tools, request counts, and expected statuses make the audit more executable.

## Read next when needed

- [`security-invariants.md`](./security-invariants.md)

