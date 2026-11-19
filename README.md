# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/ojiroaran96-ops/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ojiroaran96-ops/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python, written for the make.fun bounty [tiny-chess-01](https://make.fun/bounty/tiny-chess-01).

`main.py` is the whole engine: a 0x88 board, alpha-beta search with quiescence and null-move pruning to a fixed node budget, a transposition table, MVV-LVA ordering with killer and history heuristics, and a material plus piece-square evaluation with a king pawn-shield term. It plays through the env at `MAKEFUN_ENV_URL`, is fully deterministic (fixed node budget, no clock, no randomness), and uses only the Python standard library.
