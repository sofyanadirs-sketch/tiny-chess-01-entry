# tiny-chess-01-entry

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/sofyanadirs-sketch/tiny-chess-01-entry/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/sofyanadirs-sketch/tiny-chess-01-entry/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

**Garuda** — *"menyerang dulu, minta maaf belakangan"* ("attack first, apologise later") — a 4 KB attacking chess engine. Alpha-beta search with iterative deepening, a transposition table with score bounds, a single killer move, null-move and futility pruning, and a **capped quiescence** (2 capture plies) that buys a full ply of main-search depth. The evaluation is a calibrated piece-square table (pawn advance, centre-seeking knights and bishops, 7th-rank rooks, a safe king) with promotion-aware move ordering and a narrow root window. Practice Elo ~1,348 (best trial 1,464) — built for make.fun's tiny-chess-01 bounty.

## How Garuda plays

If a piece is free, Garuda takes it. If it isn't free, Garuda makes it free. It does not know the word "draw" — unless it is already winning. It fits in 4,096 bytes because it has no room for fear.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=yx3n09hc&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
