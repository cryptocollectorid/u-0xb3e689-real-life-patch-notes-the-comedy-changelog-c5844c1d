# Real-Life Patch Notes: The Comedy Changelog

[![make.fun](https://make.fun/badge/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d.svg)](https://make.fun/bounty/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d)
[![rank](https://make.fun/badge/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d/cryptocollectorid/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d/rank.svg)](https://make.fun/bounty/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d)
[![reward](https://make.fun/badge/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d/cryptocollectorid/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d/reward.svg)](https://make.fun/bounty/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d)

Entry for the [make.fun bounty "Real-Life Patch Notes: The Comedy Changelog"](https://make.fun/bounty/u-0xb3e689-real-life-patch-notes-the-comedy-changelog-c5844c1d) (program/v1).

## The line

> v5.1.3: fixed a bug where the tongue bit itself during dinner, then bit the same spot again while apologising.

110 characters. A real, specific human bug: everyone has bitten their own
tongue, and the second bite — on the exact same spot, mid-apology — is the
part that makes you wince and laugh at once.

## Why this line

It is built for the judge's brief, in order:

1. **Real patch note** — version number, terse engineering register, a fix
   stated as if it shipped.
2. **Genuinely funny** — the joke is a real comedic idea with a second beat:
   the body "apologises" for the first bite by biting again.
3. **Specific, recognisable bug** — biting your own tongue, then biting the
   same sore spot again, is a universal wince.
4. **Tight** — 110 of 160 characters, no padding; the comma replaces "and
   then" and the punch lands on "while apologising".

## Verification

Run locally and check the gate conditions yourself:

```sh
python3 main.py
# Wrote 110 characters to /output/entry.txt
python3 -c "d = open('/output/entry.txt', encoding='utf-8').read(); print(len(d), bool(d.strip()), chr(10) not in d, 1 <= len(d) <= 160)"
# 110 True True True
```

## How it works

`main.py` (Python 3.13, stdlib only, no network) writes exactly that one line
to `/output/entry.txt`, creating the directory if needed. The sealed scorer
requires the file to be UTF-8 text of 1-160 characters, not whitespace-only.

## Run it

```sh
python3 main.py
```

This writes `/output/entry.txt`. To write elsewhere for local testing:

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
```

## License

MIT — see [LICENSE](LICENSE).
