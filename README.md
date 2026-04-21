# Equity equivalence calculator

## What this is

An interactive tool that demonstrates why the common claim that
"5% non-dilutable equity up to €10M postmoney is equivalent to 15%
dilutable equity" is mathematically false.

The claim appears in several international term sheet references
(including AUTM guidance) and is cited by German TTOs and policy
documents as justification for specific spinout equity structures.
The two structures are not equivalent at any realistic exit
valuation — by a €500M exit, the protected stake would need a cap
30–50× larger than €10M to actually match the dilutable stake.

This tool is part of the Berlin Model project (a government-backed
standardized IP transfer framework for Berlin-Brandenburg university
and research institution spinouts).

## How it works

Single-file HTML with Chart.js loaded from CDN. No build step.

Two views:

1. **Side-by-side comparison** — plots effective final stake for
   dilutable vs protected structures across exit valuations.
2. **Breakeven cap** — computes the protection cap that would be
   required for a protected stake to actually equal a dilutable
   target stake at a given exit size.

## Model simplifications

Funding rounds are modelled at fixed postmoney checkpoints
(€5M → €15M → €40M → €100M → €250M → €600M → €1.5B → €3.5B)
with a user-controlled per-round dilution. Real rounds vary, but
the qualitative conclusion is robust across reasonable dilution
assumptions.

## Deployment

GitHub Pages works directly on the root `index.html`. No build,
no server, no dependencies beyond the Chart.js CDN.

## Editorial constraints

- Tool does not name specific institutions.
- Framing: "typical of some US-based spinout terms", not
  attributed to any named organization.
- Values 5% / €10M / 15% load as defaults because that is the
  specific equivalence claim being disproved, but the tool itself
  is neutral.

## Possible extensions

- Sensitivity view across dilution-per-round assumptions
- Cumulative capital raised as alternative x-axis
- PNG export for embedding in policy documents
- Preset scenarios drawn from published international term sheets
