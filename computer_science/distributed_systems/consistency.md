# Consistency

## Basic idea

Consistency models specify what values reads may observe given concurrent writes. They are characterised by two orthogonal properties: *safety* (nothing wrong ever happens) and *liveness* (something good eventually happens).

## Key facts

- Strict linearisability: every op appears to take effect atomically at some point between invocation and response — strongest safety, no liveness gain.
- Sequential consistency: some total order consistent with each thread's program order.
- Eventual consistency: liveness only — replicas converge if updates stop.
- Strong eventual consistency: liveness + safety — replicas that have seen the same updates are in the same state.

Consistency in the context of distributed systems revolve around two things, safety and liveness.

## Eventual consistency

Makes promises about liveness only.

## Strong eventual consistency

Makes promises about liveness and safety

## Liveness

The property that eventually something good will happen. For example saying that a system will return a result to every API call is a liveness property.

## Safety

The property states that nothing bad will ever happen. For example never returning a wrong value or electing two leaders.

