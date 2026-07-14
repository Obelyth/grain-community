# Changelog

## v0.2.0 — 2026-07-14

The **Daily Grain Check** — a daily game that turns spotting AI into a skill you
can measure.

### The game

- **Five clips a day, the same for everyone.** Swipe each one: is it real, or
  AI? Swipe a little to answer, swipe further to bet you're sure.
- **The reveal is the point.** After you call it, you find out — with the
  crowd's split ("62% got fooled by this one") and your points. Nothing's
  shown before you commit, so your gut is really your gut.
- **You get a rating.** Every clip is rated by how many people it fools, and so
  are you — guess well on the hard ones and your score climbs. Miss a "sure"
  bet and it stings. That's the honesty tax.
- **Share your run.** A spoiler-free result row (🌾 ✅❌✅✅❌ — fooled 2/5)
  you can drop in a group chat without giving away the answers.
- **No account needed to play.** Start swiping in seconds; sign in later only
  if you want to keep your points.

### Under the hood (why it's built to last)

- Points are **earned, never bought or cashed out**, and your skill rating is
  kept separate from your point balance — so trust can never be purchased.
- Every clip's answer lives **only on the server** — the app on your phone
  literally can't see whether a clip is AI until after you've guessed. No
  peeking, for anyone.

### Honesty

- The launch clips are clearly-labeled test content while the real library is
  built. Same standard as always: [docs/honesty.md](docs/honesty.md).

## v0.1.0 — 2026-07-13

First public release of the concept demo.

### The product

- **Verdict specimen card** — crowd AI-slop read (0–100 + confidence, stamped
  verdict), first flagger + spread sparkline, "why it was made" intent bars,
  sentiment strip, honest provenance line, community notes.
- **No dead ends** — known videos get curated cards; unknown ones get a
  deterministic, clearly-labeled generated card. Same link → same numbers,
  for everyone.
- **Short-link resolution** — `vm.tiktok.com` / `youtu.be`-style share links
  resolve server-side.

### Capture

- **iOS** — Share-sheet Shortcut (guided setup at `/shortcut`).
- **Android** — Web Share Target: install as PWA and Grain appears in the
  native share sheet.
- **Everywhere** — paste a link.

### Honesty

- Persistent **demo data** badge on every card; `source` field on every card's
  data; About page says plainly what's real and what's simulated.
  Policy: [docs/honesty.md](docs/honesty.md)
