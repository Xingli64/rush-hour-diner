# 🐸 Rush Hour Diner — Cooking Game

A complete, original cooking game that runs **fully offline** in a desktop browser. No dependencies, no build step: open `game/index.html` and play.

## How to play

- **Read the order** above each customer (bottom layer first).
- **Grill:** click an empty grill slot to start a patty. Take it when it flashes **PERFECT** — too early is raw, too late is burnt.
- **Fries** cook in the fryer; plate them when golden.
- **Stack** the burger on your plate in the exact order shown, add a drink if the order asks for one, then **click the customer** to serve.
- Fast, perfect serves build a **combo multiplier**. Customers who run out of patience walk out and cost a heart — lose 3 hearts and the day ends early.

## Game structure

- **3 days**, each faster and more demanding: new ingredients (cheese, lettuce, tomato, onion, egg, bacon), more drinks and fries, higher coin targets.
- Scoring: per-layer price + perfect-patty bonus + speed/combo bonus.
- Star rating per day based on coins earned vs. target.

## Repository layout (make.fun hand-in)

- `game/index.html` — the whole game (vanilla HTML/CSS/JS, zero external assets).
- `screenshots/` — real screenshots of the game running.
- `main.ts` — Node 22 hand-in program: copies `game/` and `screenshots/` to the output directory and writes `dossier.json` using the vendored library. Check locally with `MAKEFUN_OUTPUT_DIR=out node main.ts`.
- `vendor/makefun-game.ts` — make.fun's game library, vendored unmodified.
- `LICENSE` — MIT.

## Entry

Built for the make.fun bounty **“Make the best cooking game”** (https://make.fun/bounty/best-cooking-game-20261125-0137).
