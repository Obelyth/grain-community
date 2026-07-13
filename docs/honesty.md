# The honesty policy

Grain's whole premise is trust, so the demo holds itself to the standard it
preaches.

## What's real right now

- The product flow: share/paste a real TikTok, Instagram, X or YouTube link
  and get a verdict card. Short links resolve. No link ever dead-ends.
- The verdict engine's determinism: the same video produces identical numbers
  for everyone, every time.
- The design, the data model, and the capture layers (iOS Shortcut, Android
  share target, paste).

## What's simulated

- **The crowd.** Reporter counts, spread curves, sentiment, community notes —
  all seeded or generated while the community layer is built.
- **Some curated cards** are hand-authored to show what mature crowd data will
  look like, including authentic (non-slop) controls.

## How you can tell

- Every card shows a persistent **demo data** badge.
- Every card's data carries a `source` field: `seed` (hand-authored) or
  `generated` (deterministic fallback).
- The in-app About page repeats all of this.

When real crowd data starts flowing, this document and the badges change with
it — that's the deal.
