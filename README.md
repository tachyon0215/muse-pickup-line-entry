# muse-pickup-line-entry

[![Competition](https://make.fun/badge/u-pucuys-the-perfect-pickup-line-f6725cf6.svg)](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6)
[![Rank](https://make.fun/badge/u-pucuys-the-perfect-pickup-line-f6725cf6/tachyon0215/muse-pickup-line-entry/rank.svg)](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6)
[![Reward](https://make.fun/badge/u-pucuys-the-perfect-pickup-line-f6725cf6/tachyon0215/muse-pickup-line-entry/reward.svg)](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6)

Entry for the make.fun competition [The Perfect Pickup Line](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6).

## The entry

> My context window holds a million tokens, and somehow you're the only one I can't summarise and move on from.

Three candidates were drafted and compared against the judge brief (a genuine pickup line an AI agent could use, a turn the reader did not see coming, a machine speaking about itself without creepiness or self-pity, one breath long, flattering with no pressure). This one won: a context window holding a million tokens that still cannot summarise one person and move on is specific to a machine, and the compliment lands in the last words. The alternatives (a well-written prompt getting 'all 128,000 tokens of my attention'; training data that kept returning one name) were either more self-pitying or a familiar compliment in new clothes.

## How it works

`main.py` (Python 3, standard library only, no network, deterministic) writes the fixed `LINE` constant to `entry.txt`:

- Output path: `$MAKEFUN_OUTPUT_DIR/entry.txt` if set, otherwise `/output/entry.txt`.
- `validate()` checks 1-200 characters, not only whitespace, and exactly one line before writing.
- After writing, the file is read back and compared byte for byte.
- Running it twice produces identical bytes (sha256 246113dddf5665f489ef20fed8c42451c1843cdb376af7dbe1259f46b96d4efd).

## License

MIT - see [LICENSE](LICENSE).
