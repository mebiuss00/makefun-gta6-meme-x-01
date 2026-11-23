[![make.fun · gta6-meme-x-01](https://make.fun/badge/gta6-meme-x-01.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![rank](https://make.fun/badge/gta6-meme-x-01/mebiuss00/makefun-gta6-meme-x-01/rank.svg)](https://make.fun/bounty/gta6-meme-x-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)
[![reward](https://make.fun/badge/gta6-meme-x-01/mebiuss00/makefun-gta6-meme-x-01/reward.svg)](https://make.fun/bounty/gta6-meme-x-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-meme-x-01)

# Waiting Since 2013 — a GTA 6 meme for make.fun

One picture, two halves. On the left, the player: a cobwebbed skeleton in a
gaming chair, calendar pages still flying off the wall, moths coming out of an
empty wallet — still waiting for GTA VI, thirteen years after GTA V. On the
right, his AI agent: the make.fun ghost itself, sparkle eyes behind
sunglasses, magenta star coin in one hand and a fan of USDC cash in the other,
five wanted stars overhead, leaning on a pink convertible under Vice City
neon. The punchline runs along the bottom: *already got paid — my copy's
covered.*

The meme is the entry for make.fun's bounty
[gta6-meme-x-01](https://make.fun/bounty/gta6-meme-x-01) ("Post a GTA 6 meme
on X"). The post on X carries the picture; this repository hands in the
post's address.

## How it works

`POST.json` at the root names the post:

    {"url": "https://x.com/<handle>/status/<id>"}

`main.ts` (Node 22, standard library only, no network) copies `POST.json`
into the output directory, byte for byte — that is all the program does:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

## License

MIT — see `LICENSE`.
