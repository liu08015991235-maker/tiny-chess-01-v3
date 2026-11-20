# tiny-chess-01-v3

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/liu08015991235-maker/tiny-chess-01-v3/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/liu08015991235-maker/tiny-chess-01-v3/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A small chess engine in Python: 0x88 board, negamax alpha-beta with
PVS, null-move pruning, LMR, check extensions, killer/history move
ordering, a Zobrist transposition table, and quiescence over captures,
promotions and check evasions with delta pruning. Evaluation is
incremental material+PST, tapered between middlegame and endgame
(endgame king table) with a bishop-pair term. Iterative deepening
under a fixed node budget (never a clock, so replays match).

`engine_src.py` is the readable source (compact 1-space indentation
to fit the size cap); `main.py` is produced from it by the make.fun
kit compress command and is the submitted engine.

## Run it

```sh
python3 main.py
```

---
<sub>Entered on [make.fun](https://make.fun/?ref=wv1e5zfb&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
