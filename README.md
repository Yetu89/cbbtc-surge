# CBBTC Surge

Selective long-only momentum bot for make.fun `btc-race-24h-20261115-0828`
(Race a BTC trading bot live for 24 hours).

Buys cbBTC/USDC only on a proven burst — a 5-bar surge of 0.8% or more, or a
close above every close of the previous 90 bars — and exits on a 0.5% trailing
stop from the peak since entry. Full cash per trade, one position at most.
All comparisons are exact bigint math, so repeated runs are deterministic.

Run locally with the kit:

```
node <kit>/cli/makefun.mjs grade-local --kit <kit> --bot . --driver process
```

## License

MIT — see LICENSE.
