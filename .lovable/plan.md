## Goal

Rebuild `Armana_Kaizen_Baseline_Apr-Jun2026.pptx` as a data-first deck: charts and numbers carry the message, prose is cut to short bullets, and every factory (AAL, ZAL, DML, DTX, SSL) gets its own section instead of mixed portfolio tables.

## Visual system

- Light mode: off-white background (`FAFAF8`), dark grey body text (`3A3A3A`), near-black headings (`242424`).
- One accent per factory so the eye tracks the factory, not the line: AAL slate blue, ZAL teal, DML green, DTX amber, SSL plum. Muted grey for reference bars and targets.
- Fonts: Georgia headings / Calibri body. Titles 40-46pt, body 20-22pt, stat callouts 72-96pt, captions 14-16pt.
- Every slide carries a visual: bar chart, stat row, or gap chart. Max 4 bullets per slide, each ≤10 words.

## Slide structure (~17 slides)

1. **Title** — Armana Kaizen Baseline, Apr–Jun 2026, 8 of 10 lines valid.
2. **Executive scoreboard** — 4 big stats (67.1% eff, 20.3% OT, 72.9% balance, 36.7 min changeover) + 3 bullets only.
3. **Method at a glance** — 6 short fact chips (window, 2,063 records, weighting rule, no zero-fill), no paragraph text.
4. **Factory comparison** — one grouped bar chart: efficiency by factory, with 75% target line. Single slide where factories appear together, by design, as the roll-up.

Then per factory, 2 slides each (AAL, ZAL, DML, DTX, SSL):

- **Factory KPI slide** — stat cards per line (eff / OT / balance / changeover / output) + a bar chart of that factory's lines vs target.
- **Factory read slide** — 3-4 bullets max: what the data says, the lever, the verdict. Includes the factory's monthly Apr–Jun trend where records exist.

DTX gets a single slide (only 1 of 3 lines has data; the other two are "no baseline issued" — shown as a data-gap panel, not fake numbers).

Closing slides:

15. **Composite ranking** — the 8 validated lines, ranked, colour-coded by factory.
16. **90-day targets** — KPI / baseline / target / lever table, 5 rows.
17. **Wave 1 recommendation** — 2 pilot lines, 2 held out, one line of rationale each.

## Data integrity

Every figure comes from the uploaded deck only — no new numbers invented. "No data" cells stay as explicit gaps (DTX:Floor-2:L1, DTX:Floor-4:L25, AAL:Floor-3:L9 balancing/changeover) rather than being filled or dropped silently.

Note: the source deck contains one internal inconsistency — line balancing group average is quoted as 72.9% on slides 2/8 and 76.0% on slide 13. I'll use 72.9% (consistent with the per-line values) and flag it to you.

## Technical

- Generate with pptxgenjs at 16:9, native charts (not images) so numbers stay legible and editable.
- Validate the file, render slides to images, and do a visual QA pass for overflow, overlap and contrast before delivering.
- Output to `/mnt/documents/Armana_Kaizen_Baseline_Apr-Jun2026_v2.pptx` as a downloadable file (no app changes).
