# tiny-chess-01 entry v3

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
