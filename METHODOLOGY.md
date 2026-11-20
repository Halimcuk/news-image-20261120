# Methodology

## How the news was chosen

On the morning of 21 November 2026 (WIB), after 20 November had ended
everywhere on Earth, world-news roundups and live coverage for Friday
20 November 2026 were searched and cross-checked (news vertical search,
then the underlying outlets). A story was used only if at least two
independent sources reported it on 20 November 2026, and only if the
event happened — or was first reported — on that day.

That date rule mattered most this day: the biggest headlines of the
week — the Trump–Xi–Putin summit in Shenzhen, the ICJ's genocide
ruling against Myanmar, Anthropic's record IPO, the Houthi missile
strike on Riyadh's PIF Tower — all happened on Thursday 19 November,
so none of them is presented as 20 November news. What the poster
shows instead is what 20 November itself produced, including the
day-after consequences of those 19 November events:

- War, Europe: Russia's overnight missile and drone barrage on Kyiv,
  the largest of the year, hours after Putin left Shenzhen.
- Diplomacy: Trump's call to European leaders saying Putin is "tired"
  and ready for a deal — reported on 20 November by CNN and The Times.
- Climate: COP31's final day in Antalya, with fossil-fuel language
  dropped from the draft and talks extended past the deadline.
- Diplomacy, Europe: the second EU–UK summit in Brussels.
- Disaster, Asia: Cyclone Akvan's landfall on India's east coast.
- Markets: the worldwide slide in stocks as doubts about AI
  valuations spread.

One candidate was checked and dropped: Kenya's last Ebola patient
being discharged. It was widely re-shared on 20 November, but the
announcement itself was made on 11 November, so it is not a
20 November story.

Each poster line states only what the sources reported. Where casualty
figures differed slightly between outlets (8 or 9 killed in Kyiv),
the poster uses 9, the figure in the later CNN and NY Post reports,
and the summary keeps to the figures all outlets agreed on: 110+
missiles, 400+ drones, three bridges hit.

## How the image was made

The poster was generated with an AI image generator from a prompt
carrying the six headlines and summaries verbatim, in the style of a
clean newspaper front page: a navy header band, the date in large
serif type, and a 3×2 grid of cards, each with a place tag, a bold
headline and one summary line.

The first render came out at 1600×1600 and 1,192,679 bytes — over both
the 1024-pixel and 1 MiB limits — so it was downscaled to 1024×1024
with Pillow (LANCZOS) and re-saved as an optimised PNG at 623,727
bytes. The finished image was read back visually at full size and at
thumbnail size: the date, all six headlines, all six summaries and
the source footer are complete and legible, with no garbled or
invented text anywhere. No text was altered between the check and the
final file.

## The program

`main.ts` (Node 22, standard library only) copies `entry.png` to
`$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`), creating the
output directory if needed. It does no network access and writes the
same bytes on every run — verified by running it twice and comparing
sha256 hashes.
