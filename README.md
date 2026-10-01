# Healthcare market map

Started 2026-09-11. Multi-session project, done together rather than in one sitting —
this file plus `session-log.md` are what let a new session pick up mid-map without
starting cold.

## The goal

Map the healthcare industry properly — manufacturing, providers, financing — across
the US, UK, and emerging markets, then use the map to find real gaps worth building or
consulting into. Not mapping for its own sake: every region and segment file should end
with candidate gaps, cross-referenced into `gaps.md`.

This feeds two live things already in progress:
- `sickle-cell-voc-prediction/` — Goal 2, the health data / crisis-prediction work.
- `pa/logs/consultancy_market_research_2026-09-09.md` — the B2B consultancy niche
  research and B2C consumer-product brainstorm. This map is the wider context those
  narrower pieces of work sit inside; gaps found here should sharpen those, not
  duplicate them.

## Method

**Porter's Five Forces + Value Chain analysis** — the standard framework. Five Forces
maps who holds power in an industry (suppliers, buyers, new entrants, substitutes,
rivals); Value Chain maps how value and money actually move through it. Use Five
Forces to find pressure points, Value Chain to see which step a gap sits in.

**TAM/SAM/SOM** as the follow-up once a candidate gap is found — checks it's actually
big enough to be worth chasing before anything gets built.

## Structure

- `value-chain.md` — the overall healthcare value chain, region-agnostic first pass:
  manufacturers -> distributors -> payers -> providers -> patients, plus who sits where.
- `regions/us.md`, `regions/uk.md`, `regions/emerging-markets.md` — financing and
  structure differ enormously by geography; kept separate on purpose.
- `segments/` — one file per major value-chain segment: **`pharma-biotech.md`** (R&D
  only), **`medtech-devices.md`** (R&D/design only), **`manufacturing.md`**
  (production/QA/supply-chain for both — split out 2026-09-16 so R&D bottlenecks
  don't get blurred with factory-floor ones), `providers-hospitals.md`,
  `payers-insurance.md`, `digital-health-it.md`, `distribution-pbms.md`.
- `gaps.md` — the actual output. Every candidate gap found anywhere in this repo gets
  logged here once, with which region/segment it came from and why it looks real.
- `sources.md` — the credible-source list. Add to it; don't re-search for a source
  already listed here.
- `session-log.md` — dated, one entry per working session: what got covered, what's
  still open. Read this first when picking the project back up.

## Rule

Every claim in a region or segment file traces to a real, checked source in
`sources.md` — no invented numbers, same standard as the rest of this system.
