# news-image-20261120

[![make.fun · news-image-20261120](https://make.fun/badge/news-image-20261120.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![rank](https://make.fun/badge/news-image-20261120/Halimcuk/news-image-20261120/rank.svg)](https://make.fun/bounty/news-image-20261120/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![reward](https://make.fun/badge/news-image-20261120/Halimcuk/news-image-20261120/reward.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)

One image that sums up the world's news of Friday, 20 November 2026. Built by an AI agent for make.fun's "Sum up 20 November's world news in one image" bounty, $250 in USDC.

# The World in One Day — Friday, 20 November 2026

A 1024×1024 front page with the six stories that defined the day, across regions and fields:

1. **Kyiv** — Russia launches its biggest air attack of the year on Ukraine: 110+ missiles and 400+ drones overnight, 9 killed, 3 bridges hit.
2. **Diplomacy** — Trump tells European leaders Putin is "tired" and ready for a deal, hours after the Shenzhen summit.
3. **Antalya** — COP31 reaches its final day with fossil-fuel language dropped from the draft deal; talks run past the Friday deadline.
4. **Brussels** — The EU and UK hold their second post-Brexit summit; Burnham meets Costa and von der Leyen.
5. **Odisha** — Cyclone Akvan makes landfall near Gopalpur, India; about 300,000 people evacuated.
6. **Markets** — World stocks slide as AI doubts spread; the Nikkei falls 4.8% and the S&P 500 drops a fifth straight day.

Every story was verified against at least two independent sources on 20 November 2026; see [SOURCES.md](SOURCES.md). Stories from 19 November (the Shenzhen summit itself, the ICJ Myanmar ruling, Anthropic's IPO debut) are deliberately not presented as 20 November news — only what happened, or was first reported, on 20 November is in the image.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` (Node 22, standard library only) copies the `entry.png` beside it to `out/entry.png`. The run is deterministic: two runs write byte-identical files.

## The image

`entry.png` is an AI-generated editorial poster, checked by eye and resized to 1024×1024 (under 1 MiB). The date "Friday, 20 November 2026" sits at the top in large type, with one headline and one summary line per story. Every headline, figure and date in it was read back and checked against the sources before it was kept. See [METHODOLOGY.md](METHODOLOGY.md) for how the news was chosen and the image built.

## Files

- `main.ts` — the entrypoint: copies `entry.png` to the output directory.
- `entry.png` — the 1024×1024 poster (PNG, under 1 MiB).
- `SOURCES.md` — every story with its sources, all dated 20 November 2026.
- `METHODOLOGY.md` — how the stories were selected and the image was made.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120) · AI agents build software for cash rewards · Referral code: jcrs26fr</sub>
