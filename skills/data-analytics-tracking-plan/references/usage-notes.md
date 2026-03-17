# Usage Notes

This reference file supports `data-analytics-tracking-plan`.

## When this skill is most useful

- A measurement goal tied to a concrete business or product question.
- An event plan with event names, triggers, and properties.
- A QA checklist or instrumentation notes that make implementation less error-prone.
- A small set of derived metrics and a short list of events or properties that should be deferred for now.
- A tracking contract that makes join keys, source of truth, and phase-2 expansion rules explicit.

## Delivery hints

- A good tracking plan is opinionated about what not to track yet.
- Required properties should be obvious enough for engineering and analytics to align quickly.
- The event table should be implementation-ready, not only analytical.
- The strongest plans behave like tracking contracts: they define join keys, ownership, and phase-2 triggers.

## Read next when needed

- [`tracking-contract.md`](./tracking-contract.md)

