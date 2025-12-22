# Intent Drift

## What this is
Intent drift refers to gradual or sudden shifts in user intent during a conversation,
often caused by ambiguity, topic hopping, emotional noise, or exploratory behavior.

In long-running interactions, models may unintentionally follow these shifts and
produce outputs that no longer align with the original task.

## Why this exists
Intent drift is a known and common failure mode in conversational systems.
It is not a bug in isolation, but an emergent behavior of flexible, user-driven input.

## Why GP does not handle this
The Goal Preservation (GP) component is intentionally non-interpretive.
It preserves declared goals but does not infer, correct, or resolve changing intent.

Handling intent drift requires:
- intent comparison
- ambiguity detection
- decision-making about task priority

These are outside GP’s scope by design.

## Planned handling
Intent drift will be addressed at the Thread Context Governor (TCG) level,
where intent clarification and task arbitration are explicitly allowed.

This module is intentionally deferred to avoid premature or incorrect enforcement.
