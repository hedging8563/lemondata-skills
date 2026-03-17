# Tracking Contract Notes

## Source of truth

- If the event is about user intent, the frontend often owns it.
- If the event is about successful completion, billing, or background jobs, the backend should usually own it.
- Do not leave ownership ambiguous for events that power funnel conversion metrics.

## Join keys

- If a flow crosses frontend and backend systems, define the join key explicitly: user_id, session_id, anonymous_id, export_id, or similar.
- State when aliasing or identify must happen, especially across signup boundaries.
- If a correlation ID is needed, say where it is created and where it must be propagated.

## Phase 2 triggers

- Deferred instrumentation should include the trigger for adding it later, such as unexplained funnel dropoff, noisy error buckets, or strong demand for deeper attribution.
- A phase-2 trigger turns defer decisions into a roadmap, not just a no.
- If a deferred event will materially increase QA cost, say that explicitly.
