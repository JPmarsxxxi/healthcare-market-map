# Session log

## 2026-09-11 — project started
- Repo structure created: README, sources, value-chain skeleton, region and segment
  stubs.
- Sources carried over from `pa/logs/consultancy_market_research_2026-09-09.md`
  (Trellis AI, CapeStart, Sanctuaryhealth, the drug-pricing data).
- New sources found and verified: Rock Health (US digital health funding), King's
  Fund + Nuffield Trust (UK NHS structure), McKinsey Healthcare Systems & Services
  Insights (emerging markets, with the Aravind/Narayana Hrudayalaya examples).
- First-pass value chain drafted: manufacturers -> distributors/PBMs -> payers ->
  providers -> patients. Observation: everything found so far clusters around
  manufacturers, providers, and the manufacturer-patient link; payer-provider
  (claims/prior-auth) is already crowded; PBM layer and provider-to-patient
  coordination (beyond one example) are unexplored.
- Nothing in `gaps.md` yet - no region or segment has been researched deeply enough
  to log a real gap. Next session's job: pick one region or segment file and
  actually fill it in, not add more structure.

## 2026-09-11 (same day, second pass) — regions/uk.md done, first real fill-in

- Picked UK first: it's the geography he's actually operating in, connects directly
  to the Cambridge biotech conversations already planned.
- `regions/uk.md` filled in properly: the 5-layer structure (Government -> NHSE ->
  Regional Teams -> 42 ICSs -> providers), real financing numbers (~80% taxation,
  11.3% of GDP, ~25% private-sector spend, uncleanly tracked), and concretely how a
  small company actually gets into the NHS (separated test/deploy budgets, pooled
  ICS budgets, named support programmes: MedTech Venture Kickstarter, the £100M
  MedTech fund, King's Health Partners Ventures).
- Real cross-connection found, not yet a logged gap: the NHS's own stated procurement
  logic (cheap test before expensive deploy) matches the B2B consultancy pitch shape
  already recommended (CapeStart's Deep Dive-first model) — two independent sources
  converging on the same engagement shape.
- Still open in `regions/uk.md`: whether MedTech Venture Kickstarter has a live
  application window, and how ICBs actually choose small suppliers in practice.
- Next: either `regions/us.md` or `segments/pharma-biotech.md` — US has less existing
  momentum than pharma-biotech, which extends the consultancy work already done.

## 2026-09-16 — deep scrub of regions/uk.md, session 2. This is the actual standard.

- **Correction from the prior session, his call:** the 2026-09-11 UK pass was a first
  search-summary pass, not the deep scrub the project's own method promised. He caught
  this directly — "how does uk get marked done if this isn't a skim" — and he was
  right. Fixed properly this session, not just relabelled.
- King's Fund blocks direct fetching entirely (403 on every URL tried, confirmed
  again). Nuffield Trust does not — it's now the primary readable UK source.
- Two full Nuffield Trust reports read properly (not search snippets): "Where does
  the NHS money go?" and "How has the role of the private sector changed in UK
  health care?" Real figures now in `regions/uk.md` — service-by-service NHS
  spending growth 2013/14-2023/24, private-sector spend nearly doubling post-pandemic
  (£1.66bn -> £3.12bn), and the standout finding: **self-pay private healthcare
  growth in Northern Ireland (+218%) and Wales (+124%) is 5-10x England's rate
  (+20%)** — completely missed by every prior pass because nothing looked below the
  England/UK-aggregate level.
- Two candidate gaps promoted to `gaps.md`: the NI/Wales self-pay disparity, and
  dentistry's confirmed NHS-coverage shrinkage (two independent reports converge on
  it).
- Added a memory pointer (`project_healthcare_market_map.md` in this machine's
  `.claude` memory) so a fresh session on this machine finds this repo automatically
  instead of needing to be told from scratch — a real gap exposed when this session
  got continued from another machine and had no automatic route back here.
- **The standard going forward, stated plainly so it doesn't slip again:** every
  region/segment file gets this level of treatment — real reports read directly,
  not search-result summaries — before it's called done. Multi-session by design.
- Next: either finish exploring *why* NI/Wales specifically (regulatory difference?
  waiting-list severity? income?), or move to `regions/us.md` / `segments/pharma-biotech.md`.

## 2026-09-17 — segments/pharma-biotech.md done, all six method steps run properly

- First segment file (as opposed to region file) done, and the first time all six
  steps of the stated method were run in full, one at a time, with a discussion
  after each — matches his explicit request for a stated plan before executing and
  a pause after every step.
- Split `pharma-biotech.md` and `medtech-devices.md` apart from `manufacturing.md`
  first (his call, 2026-09-16) — R&D bottlenecks and factory-floor bottlenecks are
  different people and problems.
- Real findings, all six steps: buyer is small-mid biotech R&D teams (findable via
  One Nucleus, 500+ Cambridge members, and BIA, 600+ UK-wide); incumbent tools
  Benchling/Dotmatics have real, named user friction (thin regulatory support, poor
  module integration); real funded competitors exist (Scoop, Alchemy, Adaptyv, edison
  scientific, Domino Data Lab) but ALL of them chase big pharma (GSK, AstraZeneca,
  "top 5 pharma") — none target small teams; the underlying problem (manual research
  curation can't keep pace with publication volume) is stated repeatedly in the
  scientific literature itself, not assumed; a live, named, real target already
  sits in his own job data — **Epoch Biodesign**, hiring for exactly this kind of
  work right now.
- **Conclusion: the niche already recommended (agentic automation for small biotech
  R&D teams) is CONFIRMED by this deep dive, not replaced by a new idea.** Promoted
  to `gaps.md` as the strongest-evidenced gap in the whole project so far.
- Also gave him a plain, concrete "what does this look like day to day" explanation
  (a scientist losing up to 3 days/week to manual literature screening; a lab
  technician manually cleaning raw data every experiment) — he asked directly because
  the company-name-heavy version wasn't landing. Worth remembering: he wants the
  human-scale version alongside the evidence, not instead of it.
- Next: `medtech-devices.md` (R&D) is the natural next segment given the pharma-biotech
  momentum, or `manufacturing.md` to test the "might just reinforce park niche 2"
  hypothesis stated when it was split out.

## 2026-09-17 (same day) — PAUSED HERE. Went concrete instead of continuing the map.

**Why paused:** deep-dived the pharma-biotech segment down to 8 named real
companies (Epoch Biodesign, Clock.bio, Crescendo Biologics, F-star, Healx, Cyted,
BenevolentAI, Immutrin — full profiles in `segments/pharma-biotech.md`) to make the
abstract niche concrete. From there he asked "what tool would these guys actually
use" — which turned into picking and scoping an actual first build (a gel/blot
band-quantification tool) rather than continuing sideways across the segment grid.

**What came out of that detour, in case a session needs it:**
- Full competitive + patent check done on the gel/blot idea — written up properly
  in `C:\Users\User\gel-blot-analyzer\BUILD_BRIEF.md`, a separate repo, not this one.
  Short version: ImageJ (manual, universal), Phoretix 1D (small 10-person company,
  automated, desktop-only, hidden pricing), GelBox (free, modern, academically
  legitimate, but only 3 GitHub stars — real but essentially unused). A Quest
  Diagnostics patent (US 11686703) covers a specific diagnostic pattern-matching
  method, not plain band detection/measurement — read the actual claims, not just
  the description, before concluding that.
- **A real process lesson worth keeping for every future company/product check in
  this whole project:** the first pass on gel/blot ("no proper SaaS exists") came
  from another chat and was wrong — a real competitor (Phoretix 1D) existed and
  wasn't found until asked to cross-check. **Never carry a claim from another
  session into this map without verifying it here first.**
- Decision: build it, small v1, bands detected automatically by default, no
  install, batch upload, one-click export. Patent boundary: never correlate a
  lane's pattern against a stored reference database to classify it — plain
  detection and measurement only.
- Separately, not part of this map: built a 5-part audio drill on data cleaning
  (source: Ilyas & Chu, "Data Cleaning," A C M Books) in his PA repo's
  book-to-audio format, for building the underlying technical skill this whole
  niche depends on.

**Where to pick this map back up:** `medtech-devices.md` or `manufacturing.md`,
exactly as planned before the detour — the detour didn't change the plan, it just
came first.
