# makefun-tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Glauciky/makefun-tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Glauciky/makefun-tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 3,924-byte Python chess engine: 0x88 board, negamax alpha-beta with iterative deepening to a fixed node budget (120,000 nodes, ~2 s/move), quiescence search, transposition table, null-move pruning, late-move reductions, MVV-LVA + killer-move ordering, and tapered material + piece-square evaluation. Local practice trials (6 games each): Elo 1364 / 1545 / 1654, mean 1521 — above the 1,154 final floor and the ~1,365 house baseline mean. Deterministic: fixed node budget, no clock, no randomness.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:18080 python3 main.py
```

`main.py` is the whole engine (Python 3.13, standard library only). It plays through the make.fun env: `POST /game`, `POST /move`, `POST /resign`.

---

<sub>Entered on [make.fun](https://make.fun/?ref=hst5m5ez&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
