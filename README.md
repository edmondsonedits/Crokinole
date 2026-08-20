# Crokinole Arcade

A mobile-first browser Crokinole game with a tournament-style Classic mode plus digital-only arcade modes.

## Play

GitHub Pages: `https://edmondsonedits.github.io/Crokinole/`

Controls: touch/click the highlighted shooting arc, drag backward like a slingshot, and release. A longer pull creates more power.

## Modes and systems

- **Classic** — 1-player CPU or local 2-player Crokinole with opponent-contact / play-to-the-middle shot validation.
- **Trick Shot Challenges** — 12 escalating scenarios with persistent 1–3 star ratings.
- **Style Shots** — detects peg banks, bank masters, chain reactions, contact-20s, and perfect 20s; style points persist locally.
- **Arcade Chaos** — random board modifiers including ice, crosswind, moving/missing pegs, giant/tiny 20 holes, no-20 rounds, double tens, heavy discs, and super-bounce rounds.
- **Adventure** — a roguelite run through five opponents/bosses with lives, upgrade choices, and persistent run wins.
- **Bosses** — The Rookie, The Carpenter, The Iceman, The Sniper, and The Giant each change AI or board behavior.
- **Special discs** — Heavy, Glass, Ghost, Sticky, Spring, and Magnet discs alongside normal discs.
- **Survival** — enemy discs advance toward the centre after every shot; clear waves before your lives run out.
- **4-Player Free-for-All** — local hot-seat play with Red, Blue, Green, and Gold shooting from four sides.
- **Daily Challenge** — deterministic daily three-shot scenario with a locally saved best score.
- **Customization** — Maple, Walnut, Northern Ice, Neon Arcade, and Cottage Pine boards plus Classic, Glass, Stone, and Neon disc skins.
- **Replay / slow motion** — records the last shot and replays its physics trajectory.
- **Crokinole Golf** — a nine-hole course with target cups, bumpers/hazards, and stroke scoring.

## Technical notes

The project remains dependency-free at runtime. The full tested game is compressed into six payload chunks and loaded by `index.html`; this keeps the GitHub connector deployment reliable while preserving the complete standalone Canvas/Web Audio game. The same loader is mirrored under `/docs` so either supported GitHub Pages branch source can serve the current build.

Progress, challenge stars, customization, daily bests, adventure wins, and style points are stored with `localStorage` on the device.
