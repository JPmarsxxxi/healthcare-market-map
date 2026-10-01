# UK — NHS structure and financing

Researched 2026-09-11. Sources: NHS England's own structural explainer, The King's
Fund (via search, direct fetch was blocked). See `sources.md` for links.

## The structure — five layers, money flowing down, care flowing up

1. **Government** — sets overall NHS funding via taxation and National Insurance.
   Secretary of State + Department of Health and Social Care set top-level priorities.
2. **NHS England (NHSE)** — the single national body. Oversees funding, planning,
   delivery, performance for the whole of England. Commissions some services
   nationally, distributes most funding downward.
3. **7 Regional Teams** — manage quality/performance regionally, work with ICSs.
4. **42 Integrated Care Systems (ICSs)** — established July 2022, the current
   structural model. Each ICS = Integrated Care Board (commissioning) + Integrated
   Care Partnership (strategy) + local authorities + Primary Care Networks + provider
   collaboratives, all covering a defined local population.
5. **Providers** — hospitals, GP practices, ambulance services, mental health
   organisations, pharmacies — funded through contracts with ICBs. Primary Care
   Networks group GP practices (30-50k patients) with community/mental
   health/pharmacy to deliver care "closer to home."

**Money flow, simply:** Government -> NHSE -> ICSs -> local providers, allocated by
regional/local need.

## Financing, the real numbers

- **~80% of NHS funding comes from general taxation and National Insurance** — not
  a mixed insurance-based system like the US.
- **UK spends 11.3% of GDP on health (2022)**, up from 9.9% pre-Covid.
- ⚠️ **~25% of NHS spending arguably flows to the private sector already** — via GP
  practices, pharmacy, optical, dental, and contracted services. This is a genuinely
  fuzzy number: King's Fund itself notes central bodies don't hold clean data on
  individual contracts, especially small ones. **Practical read: private/contracted
  providers already do real, if uncounted, NHS-funded work — the door is not closed
  to non-NHS entities, it's just poorly tracked.**

## How a small company/vendor actually gets in — this is the useful part for you specifically

The NHS's own 2025-26 strategy explicitly frames itself as needing to work
*with* industry, not just buy from it. Concrete, real routes found:

- **Separated testing vs deployment budgets** — the NHS's own stated approach: fast,
  cheap testing informs a procurement decision before the slower, expensive
  deployment/training/service-redesign spend commits. **This is structurally similar
  to the "cheap discovery pilot before a real contract" model already found in the
  consultancy research (CapeStart's Deep Dive phase) — the NHS's own procurement
  logic matches the pitch shape already recommended.**
- **Pooled multi-provider budgets** — several ICSs/providers can pool budgets for one
  shared problem, delegated to a single innovative supplier. Means a solution doesn't
  need to sell to one hospital at a time necessarily.
- **Named support programmes for small companies specifically:**
  - **MedTech Venture Kickstarter** — 4-month structured programme, helps new medical
    devices/ventures with NHS adoption and procurement knowledge.
  - **£100M MedTech and medicines start-up investment fund** (2026).
  - **King's Health Partners Ventures** — the UK's first NHS-backed venture fund.
  - Innovate UK connections referenced alongside these.

## Candidate observations (not yet promoted to `gaps.md` — need more evidence first)

- The NHS's stated procurement logic (test cheap, prove it, then deploy) is
  structurally the same shape as the B2B consultancy pitch already recommended —
  worth checking whether any of the named support programmes above (MedTech Venture
  Kickstarter especially) are a real, low-cost entry point for a solo operator, not
  just for funded medtech startups.
- The ~25% private-sector NHS spending figure being "poorly tracked" by the NHS's own
  admission suggests small/niche contracted work is normal and not unusual — worth
  weighing against the assumption that only big vendors can sell into the NHS.

## Still open
- Exactly how ICBs choose which small suppliers to contract with, practically.
- Whether the MedTech Venture Kickstarter or similar programmes have any live cohort/
  application window right now.
- Comparison against `regions/us.md` and `regions/emerging-markets.md` once those
  exist — does single-payer structure make a UK gap easier or harder to find than a
  US one?

---

## Deep scrub, session 2 (2026-09-16) — real Nuffield Trust reports, not search summaries

_King's Fund blocks direct fetching entirely (403 on every URL tried). Nuffield Trust
does not — read two of their actual reports properly this time. This is the standard
this whole file should have been researched to from the start._

### Where NHS money actually grew or didn't, 2013/14-2023/24 ("Where does the NHS money go?", Gainsbury & Julian)

- **Overall NHS spending grew 3.1%/year in real terms** — about half a point below the
  long-term historical average, i.e. funding growth has been slowing.
- **Fastest-growing:** mental health (+5.3%/yr, share of budget 8% -> 9%), ambulance
  services (+5.2%/yr), acute hospital care (+4.4%/yr).
- ⭐ **Slowest, and the real finding:** community health care grew just **0.5%/year**
  over seven years (share fell 8% -> 7%); the local authority public health grant fell
  **-21% in real terms**; community pharmacy, optometry and dentistry **fell** in real
  terms outright. GP primary care grew 3.3%/yr but held a flat ~8% share throughout.
- **The actual policy failure, stated by the report's own authors:** services meant to
  deliver "closer to home" care — community, primary care, public health — collectively
  grew at **under 0.5%/year combined**, directly contradicting the stated policy goal
  of shifting care out of hospitals. **Money keeps going to hospitals despite the
  policy saying it shouldn't.**
- **NHS trust outsourcing to private/voluntary providers rose** 1.2% -> 1.9% of acute
  funding (2016/17-2022/23); **mental health outsourcing nearly doubled**, 2.9% -> 5.1%.

### How the private sector's role has actually changed ("How has the role of the private sector changed in UK health care?", Dayan, Gainsbury & Bagri)

- **NHS trusts' own spending on private care nearly doubled post-pandemic:** £1.66bn
  (2019/20) -> £3.12bn (2022/23), **+88%**. Driven by waiting-list desperation, not
  ideology or efficiency — the authors' own words: "driven mainly simply by a search
  for somebody to deliver care when there is far too little."
- **NHS patients treated in private hospitals rose** 5.6% -> 7.5% of all planned
  admissions; NHS patients in NHS hospitals fell 88% -> 85%. Current quarterly data:
  privately-provided NHS-funded care now runs **over 100,000 patients/week**, up
  30,000/week since tracking began in 2021.
- ⭐ **The regional disparity is the standout, unresearched-anywhere-else finding:**
  self-funded (out-of-pocket) private care spend, Sept 2019 -> Sept 2023:
  - **Northern Ireland: +218%**
  - **Wales: +124%**
  - **Scotland: +80%**
  - **England: +20%**
  - UK overall: +32%

  **England — the market everyone defaults to researching — has by far the SLOWEST
  self-pay growth of the four UK nations.** Northern Ireland's growth is more than
  10x England's. This has not shown up in anything researched so far because nothing
  before this looked below the England/UK-aggregate level.
- **Dentistry specifically shows real, outright NHS coverage shrinkage** — matches the
  falling-real-terms figure from the funding report above. Two independent reports
  converge on dentistry being a genuine, currently-underserved gap.
- The authors' own warning: this growth is "allocated purely based on the ability to
  pay," not competitive improvement — a real equity concern, worth being aware of
  before treating this purely as "opportunity."

### Promoted to `gaps.md`
Two candidates now cross the evidence bar (see `gaps.md` for the full entries):
1. Northern Ireland / Wales self-pay healthcare growth — 5-10x England's rate, entirely
   unresearched by anything found so far because research defaults to England.
2. Dentistry — confirmed shrinking NHS coverage from two independent reports.

### Still open, updated
- Why NI/Wales specifically — regulatory difference, NHS waiting-list severity
  difference, income difference? Not yet known, needs its own research pass.
- ICB small-supplier selection and MedTech Venture Kickstarter's live status — still
  unanswered from session 1.
