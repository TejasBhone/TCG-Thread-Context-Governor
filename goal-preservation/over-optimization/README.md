# Over-Optimization

## What this is
Over-optimization occurs when a system excessively refines, restructures,
or improves outputs beyond what the task requires.

This may result in:
- unnecessary complexity
- loss of user intent
- reduced clarity
- increased latency

## Why this exists
Modern models are incentivized to be thorough and polished.
Without boundaries, this can lead to solving problems the user did not ask for.

## Why GP does not handle this
GP does not evaluate output quality, efficiency, or optimality.
Its role is limited to preserving the existence of a declared goal.

Deciding when “good enough” is sufficient requires:
- output evaluation
- relevance judgment
- user preference inference

These functions are outside GP’s mandate.

## Planned handling
Over-optimization controls will be handled by TCG,
where output shaping and scope restraint are explicitly permitted.

This allows GP to remain minimal and non-opinionated.
