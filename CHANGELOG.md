# Changelog

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
