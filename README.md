# Equity equivalence calculator

## What this is

An interactive tool that demonstrates why the common claim that
"5% non-dilutable equity up to €10M postmoney is equivalent to 15%
dilutable equity" is mathematically false.

The claim appears occasionally in documents comparing typical UK or international 
spinout terms with typical US terms ([1](https://www.cancerresearchhorizons.com/news-and-events/our-articles/uk-spinout-review-moving-beyond-equity), [2](https://www.timeshighereducation.com/blog/uks-inferiority-complex-around-university-spin-offs-misguided), [3](https://techventures.columbia.edu/term-sheet-recommendations-for-launching-university-startups), [4](https://www.bihealth.org/fileadmin/Charit%C3%A9_BIH_Innovation/CBI_Dateien/2026-03-25_Gr%C3%BCndungsnavigator_final.pdf)).
The two structures are not equivalent at any realistic exit
valuation — by a €500M exit, the protected stake would need a cap
many times larger than €10M to actually match the dilutable stake.

This tool is part of the Berlin Model project (a standardized IP transfer 
framework for Berlin-Brandenburg university and research institution spinouts).

## How it works

Single-file HTML with Chart.js loaded from CDN. No build step.

It includes: 

1. **Side-by-side comparison** — plots effective final stake for
   dilutable vs protected structures across exit valuations.
2. **Breakeven cap** — computes the protection cap that would be
   required for a protected stake to actually equal a dilutable
   target stake at a given exit size.

## Model simplifications

Funding rounds are modelled at fixed postmoney checkpoints
with a user-controlled per-round dilution. Real rounds vary, but
the qualitative conclusion is robust across reasonable dilution
assumptions.
