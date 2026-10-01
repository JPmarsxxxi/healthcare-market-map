# Healthcare value chain — region-agnostic first pass

Status: skeleton, 2026-09-11. Fill in as regions/segments get researched — this file
is the map of *how the pieces connect*, the region files are *how each piece actually
works in that country*.

## The chain, roughly, money and product both flowing through it

```
Manufacturers — R&D/discovery  (pharma-biotech.md, medtech-devices.md)
        |
Manufacturers — production/QA  (manufacturing.md, split out 2026-09-16)
        |
   Distributors / wholesalers  (+ PBMs sit here on the drug side in the US specifically)
        |
   Payers (insurance, government schemes, out-of-pocket)
        |
   Providers (hospitals, clinics, pharmacies, labs)
        |
   Patients
```

Data and information flow the other way too (EHRs, claims data, trial data), and
several players sit *across* the chain rather than at one point in it — health IT
vendors (Epic etc.), PBMs, and increasingly the "forward deployed" AI vendors already
found in the consultancy research sit between providers and payers, or between
manufacturers and patients.

## Where the consultancy/consumer research already done sits on this chain

- Niche 1 (data pipelines), Niche 3 (agentic R&D automation) — **inside** manufacturers
  (biotech R&D), not touching payers or patients.
- Niche 2 (ML auditing) — sits at the manufacturer/regulator interface (GxP compliance).
- Prior-auth automation (Trellis AI etc., ruled out as crowded) — sits between
  **payers and providers**.
- Sanctuaryhealth — sits **inside providers** (clinic operations).
- The consumer drug-pricing/PAP ideas (Part 4 of the consultancy doc) — sit between
  **manufacturers and patients**, bypassing payers/providers largely.

**Observation, provisional:** everything found so far clusters around manufacturers,
providers, and the manufacturer-patient link. The payer-provider link (claims,
prior-auth) is crowded. **Not yet properly explored: the distributor/PBM layer, and
providers-to-patients directly (scheduling, referrals, care coordination) outside the
one Sanctuaryhealth example.**

## Open questions for this file
- Where do PBMs (US-specific) actually sit and how much of the money do they hold?
- Does the UK's single-payer (NHS) structure collapse several of these steps into one,
  changing where a gap could sit?
- What does this chain look like in an emerging market with much lower insurance
  penetration and more out-of-pocket payment?
