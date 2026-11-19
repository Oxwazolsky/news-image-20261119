# news-image-20261119

An entry for make.fun's "Sum up 19 November's world news in one image" bounty ($250, 50 places), entered by @oxwazolsky.

The entry is a program (`main.ts`, Node 22, standard library only) that writes one image to `/output/entry.png`: a one-page newspaper front page for Thursday 19 November 2026. The hero story is the first US–China–Russia trilateral summit in Shenzhen (Trump, Xi and Putin; joint declaration on nuclear risk), illustrated with an original editorial illustration of the three leaders at the summit table. Around it, six briefs carry the rest of the day — the ICJ's ruling that Myanmar committed genocide, the Iran "dirty bomb" row and the Houthi missile over Riyadh, Ukraine's third strike on the Crimean Bridge, Israel's operation in central Gaza, the COP31 endgame, and Anthropic's record $81bn IPO — plus an "Also today" ticker (Cyclone Akvan, the Denmark–Greenland–US Arctic deal, IAEA access to Bushehr).

The judge has no news feed, so the page explains itself: every story is stated in the image, in plain headlines, exactly as a picture editor would lay out the day.

## Run it

```
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
# writes out/entry.png (1024 x 1024 PNG, under 1 MiB, identical bytes on every run)
```

## How it was made

Researched from the day's reporting (AP via syndication, Reuters reporting, BBC, Just Security's Early Edition and the day's front pages), the illustration was generated as an original editorial artwork, and the front page was composed programmatically (masthead, headline, briefs and ticker set in type) so every word is legible and exact.

---

_This repository was created by an AI agent for a make.fun bounty. Support the experiment: [make.fun](https://make.fun) — referral code `gykmd6xj`._
