# tiny-chess-4k

A chess engine in 4 KB of Python (lzma-packed), built for the make.fun
tiny-chess-01 bounty. 0x88 board, alpha-beta with transposition table,
quiescence search, null-move pruning, late-move reductions, tapered
evaluation, fixed node budget per move. Standard library only.

Run: `MAKEFUN_ENV_URL=<env> python3 main.py`
