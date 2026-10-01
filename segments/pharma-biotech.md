# Pharma / biotech segment — R&D and discovery only

Status: **deep scrub done, 2026-09-17.** All six method steps run properly, real
sources throughout — see below and `sources.md`.

**Scope:** research and discovery only — labs, research teams, drug/therapy discovery
and development. Manufacturing is a separate file — `segments/manufacturing.md`.

## The day-to-day problem, made concrete (so this isn't abstract)

Two real, ordinary examples of the actual bottleneck, not a company name:
- **A scientist needs to know if anyone's published anything relevant.** A search
  returns ~200 papers. Reading title+abstract on each to narrow it down takes a full
  day; properly reading the ~10 that matter takes another day or two. **Up to 3 days
  of a scientist's week, gone, before their own work even starts** — repeated every
  few weeks whenever a new question comes up.
- **A lab experiment produces a raw data file** — unlabelled, some missing values,
  some sensor-glitch errors. Someone manually cleans and reformats it before anyone
  can analyse it. An hour or two, **every single time an experiment runs.**

Neither of these is one big dramatic problem — they're small, repeated chunks of time
that never register as "a problem" on anyone's radar, but add up week after week. A
small team has nobody whose job is "fix this"; it just eats into scientists' actual
science time. That's exactly why it's sellable — a few days of build time removes a
recurring weekly cost, permanently.

## Step 1 — Five Forces

- **Buyer:** small-mid biotech R&D teams. Findable via YC's company directory
  (filterable "Biotech"), **One Nucleus** (Cambridge/London, 500+ members), **BIA**
  (UK-wide, 600+ members).
- **Suppliers (incumbent tools already in use):** **Benchling** and **Dotmatics**
  dominate. Real, named user friction, checked on Capterra/G2: Benchling's own users
  say its "regulatory submission capabilities are thinner than its R&D story";
  Dotmatics users report real pain with its different modules not integrating well.
  **These gaps are concrete wedges** — specific things the big incumbent platforms
  don't cover well.
- **New entrants:** **Scoop** (YC) automates regulatory document prep (CTDs, CSRs,
  INDs, BLAs). **Alchemy** (YC) automates lab image analysis, 90%+ claimed time
  reduction — not FDA-approved (pursuing 510(k) clearance, confirmed directly),
  currently positioned purely as a research tool, same lane you'd be in.
- **Substitutes:** a team just using ChatGPT themselves, free. Means the pitch has to
  be "the specific thing already built for you," never "AI could help with this."
- **Rivalry:** searched directly for a named biotech-R&D case study from the four
  boutique AI-consulting agencies found earlier (Vstorm, Markovate, Pravaah, Azumo) —
  found none. Absence of evidence, not proof of absence, but a real signal this
  narrows out of the generic "agentic AI consulting" crowding once you get this
  specific.

## Step 2 — value chain placement

Sits at the very first step of the whole healthcare chain — before manufacturing,
distribution, payers, providers, or patients. Nothing here touches money changing
hands for treatment or care. The cleanest, lowest-complication position on the
entire map.

## Step 3 — bottleneck-finding, three channels

- **Job-posting mining (own DB):** **Epoch Biodesign** (real, funded, plastic-
  recycling biotech) is hiring a Scientific Data Engineer right now specifically to
  build the data pipelines connecting lab biologists to their computational systems
  — a live, named target doing exactly this. A separate "Founding Scientific Data
  Scientist" role at a confidential AI-drug-discovery startup exists purely to keep
  training data clean enough to trust — confirms data-quality curation is a real,
  currently-staffed cost.
- **"Who's already doing this":** the exact target role already exists at real
  companies — **Adaptyv, edison scientific, Domino Data Lab** are all hiring
  "forward deployed" engineers specifically for biotech/life-sciences R&D. Platform
  companies already selling into this space too: Scispot, Ardigen, DeepLife.
- **Is the pain real, not a hunch:** yes, and it's stated repeatedly in the
  scientific literature itself, not just anecdote — manual curation of published
  research cannot keep pace with publication volume, and funding bodies won't pay
  for a bigger human curator workforce to fix it. A structural, admitted gap.

## Step 4 — competitive check

Checked whether the named competitors (Scoop, Alchemy, Adaptyv, Domino Data Lab)
actually chase small teams or only big ones. **They chase big ones.** Domino's named
customers: GSK, AstraZeneca. Adaptyv's are "top 5 pharma" and frontier AI labs.
**Nobody found is specifically going after the small, under-resourced team** — same
gap pattern as Sanctuaryhealth in hospitals. The opening isn't "nobody does this
work," it's "nobody's bothering with the small ones."

## Step 5 — TAM/SAM/SOM

- **Realistic serviceable pool, Cambridge specifically:** One Nucleus, 500+ member
  organisations (biotech/pharma/medtech/diagnostics + service providers).
- **UK-wide:** BIA, 600+ members.
- **Obtainable, for one person starting from zero:** doesn't need the whole UK — even
  a small fraction of 500+ local organisations being small enough to say yes without
  procurement is far more than needed to land a first client.

## Step 6 — conclusion

Real, documented, structural problem. Real proof people already get paid to fix
versions of it. Everyone doing it at scale chases big pharma. A genuine, large,
physically local (Cambridge) pool of small teams nobody big is individually chasing.
**This segment holds up — the niche already recommended is confirmed, not just
asserted.**

## Promoted to `gaps.md`
- Small/under-resourced Cambridge-area biotech R&D teams, specifically the gap
  between Benchling/Dotmatics' coverage and what small teams actually need (thin
  regulatory-doc support, poor module integration) — B2B, matches the already-
  recommended niche exactly.

## Named company deep-dive, 2026-09-17 — 8 real profiles, not hypothetical

Picked from One Nucleus's Cambridge directory + own job-posting mining. Real employee
counts, funding, and stage where found — this is what "small, reachable, real
bottleneck" actually looks like as named companies, not a category.

| Company | Size | Stage/funding | The concrete pinch point |
|---|---|---|---|
| **Epoch Biodesign** | small, funded | venture-backed, building a demo plant | Hiring a Scientific Data Engineer right now to connect lab biologists' work to computational systems — the exact bottleneck, live, today. |
| **Clock.bio** | small | $4M, launched 2023 | One single-cell CRISPR screen generated **20 terabytes of data** from 3M cells. A team this size has no business having a dedicated big-data infrastructure team — and almost certainly doesn't. |
| **Crescendo Biologics** | **12 employees** | has active collaborations with **Takeda and BioNTech** | 12 people managing the data/reporting rigor two giant pharma partners expect. A tiny team punching miles above its weight administratively. |
| **F-star Therapeutics** | **39 employees** | clinical-stage, 4 drugs in the clinic | Once a drug's in clinical trials, regulatory documentation volume explodes — but the team hasn't grown to match. |
| **Healx** | small-mid | AI drug discovery for rare disease | Already hiring an "Agentic AI Engineer (life sciences)" internally — not itself a target for this exact fix, but hard proof the market pays for it, and worth knowing/learning from directly. |
| **Cyted** | growing fast | $44M Series B | Own words: "still work like a startup... we build as we go." A fast-scaling diagnostics company almost certainly has messy, patched-together data pipelines from its early days. |
| **BenevolentAI** | 69 employees | cut staff 19% recently, funding pressure | A company under real financial strain, with existing AstraZeneca/Merck partnership obligations still running — a genuinely cost-conscious buyer, which cuts both ways: motivated to save money, but may also have frozen new spend entirely. |
| **Immutrin** | — | **$87M Series A**, just raised | Heading toward a clinical proof-of-concept study — about to hit the exact regulatory-documentation cliff F-star is already on. Early enough to build the right process now rather than fix a mess later. |

**What this table is actually for:** these are not "companies to cold-email today."
They're **proof that the abstract bottleneck (steps 1-6 above) is real at specific,
named, checkable places** — so when a coffee-chat conversation happens with someone
adjacent to this world, there's a concrete reference point ("I've been looking at
teams like Crescendo — 12 people managing Takeda-level data expectations — is that
the kind of thing you run into?") instead of a vague pitch.
