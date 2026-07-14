# How Grain works

## The Daily Grain Check

Every day, five short clips — the same five for everyone. Your job: call each
one **real or AI**. Swipe a little to make a quick call, swipe further to bet
you're sure. You only find out after you commit, so there's no peeking and no
crowd to follow — just you and your eyes.

Then the reveal: were you right, how many other people got fooled, and your
points. Do well on the clips that fool most people and your **detection rating**
climbs — a real, earned measure of how good you are at spotting AI. Miss a
confident bet and it costs you. At the end you get a spoiler-free result row to
share.

Two rules keep it honest and keep it fair:

- **The answer lives only on the server.** Your phone can't see whether a clip
  is AI until you've already guessed — so nobody can cheat, and the crowd data
  stays real.
- **Points are earned, never bought**, and your skill rating is kept separate
  from your point balance. You can't buy your way to trusted.

This is the seed of the bigger idea: a crowd of people with *measured*
judgment, whose collective read on a video means something precisely because
they've proven they can tell.

## The verdict card

Every checked video gets a **specimen card**:

- **Crowd read** — a 0–100 AI-slop likelihood with a confidence level, stamped
  with the verdict: `AI SLOP`, `LIKELY AI`, `CONTESTED`, or `AUTHENTIC`.
- **Who caught it** — the first flagger and how many joined, with a spread
  sparkline showing how fast the reports moved.
- **Why it was made** — the crowd's read on intent: trick, sell, rage-farm,
  entertain, or inform.
- **Mood** — how people felt about it (angry, amused, fooled, impressed).
- **Provenance** — an honest line about what the file's metadata does and
  doesn't prove (C2PA content credentials when present — which is rare).
- **Community notes** — the sharpest observations, ranked by helpfulness.

## Crowd-first, on purpose

Detection algorithms are already losing the arms race against generative
video, and that gap only widens. Grain treats **the crowd as the primary
signal** — thousands of eyes catch what one classifier misses — with
provenance and (soon) model-assisted hints in a supporting role, clearly
labeled as such.

## The pipeline

```
share / paste a link
   → canonical id        (one video = one id, across share-link variants)
   → seed or generated   (curated card if we have one; deterministic
                          generation if not — same numbers for everyone)
   → the verdict card
```

No link ever dead-ends: an unknown video gets a believable, clearly-labeled
generated card rather than an error page.

## Every surface is a thin shim

The iOS Shortcut, the Android share target, and the paste box all do exactly
one thing: hand a link to the same pipeline. That's deliberate — it keeps every
future surface (browser extension, native apps) cheap to add and identical in
behavior.
