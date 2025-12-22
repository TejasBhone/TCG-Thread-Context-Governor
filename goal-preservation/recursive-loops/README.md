# Recursive Loops

## What this is
Recursive loops occur when a system repeatedly revisits the same concepts,
questions, or clarifications without meaningful progression.

This can happen due to:
- unclear goals
- repeated user uncertainty
- over-validation by the model
- excessive self-referencing

## Why this exists
Recursive behavior is a natural risk in systems that aim to be helpful,
polite, or flexible over long conversations.

Left unmanaged, it can lead to stagnation or user frustration.

## Why GP does not handle this
GP does not track conversational history beyond the locked goal reference.
It has no concept of repetition, progress, or conversational state depth.

Detecting and breaking loops requires:
- turn-level memory
- progress heuristics
- intervention logic

These are explicitly excluded from GP.

## Planned handling
Recursive loop detection is planned as a higher-order control concern
within TCG, where conversation structure and progression can be evaluated.

This separation ensures GP remains predictable and stable.
