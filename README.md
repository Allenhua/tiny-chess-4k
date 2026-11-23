# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Allenhua/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Allenhua/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python (lzma-packed), built for the make.fun
tiny-chess-01 bounty: https://make.fun/bounty/tiny-chess-01
0x88 board, alpha-beta with transposition table,
quiescence search, null-move pruning, late-move reductions, tapered
evaluation, fixed node budget per move. Standard library only.

Run: `MAKEFUN_ENV_URL=<env> python3 main.py`

Local practice vs the house ladder (trial-0, 30k nodes): W depth-2,
L depth-3, D depth-4, L nodes-100k, D nodes-250k, L nodes-500k
(~1200 Elo). This build raises the budget to 45k nodes, adds a tapered
king evaluation and repetition avoidance.
