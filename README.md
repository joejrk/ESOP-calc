# IRA land purchase & Roth conversion calculator

`ira-land-calculator.html` is a single self-contained page — no build step, no external
dependencies. Open it directly in a browser, or host it anywhere static.

It models moving a traditional IRA into land inside a self-directed IRA, then converting an
equal slice of the acreage into a Roth IRA each year from the purchase age up to the age
conversions end.

## Inputs

Starting land value, acreage, purchase age, age conversions end, salary (MFJ), annual land
appreciation rate, and annual appraisal cost. Everything recalculates as you type.

## Outputs

- Year-by-year schedule: acres converted, $/acre that year, slice value, tax owed, and the age
  that slice becomes usable.
- Running totals: land value at the end age, total conversion tax, effective tax rate, net kept.
- Lump-sum comparison: withdrawing the full starting value at the purchase age with ordinary
  income tax plus the 10% early-withdrawal penalty.
- All-in cost including appraisals.

## Tax model

2026 federal married-filing-jointly brackets: 10% to $24,800; 12% to $100,800; 22% to $211,100;
24% to $403,300; 32% to $512,450; 35% to $768,700; 37% above. Each year's tax is the marginal
cost of the conversion — tax on salary plus the slice, minus tax on salary alone.

A converted slice becomes penalty-free at conversion age + 5, capped at 60: past 59½ the
conversion 5-year rule no longer gates access.

State taxes, NIIT, deductions, credits, and phase-outs are not modeled.

## Hosting

Self-contained, so any of these work: paste the file's contents into a Google Sites *Embed code*
block, serve it from GitHub Pages and embed by URL, or drop that URL into Notion with `/embed`.

## Caveat

General, publicly available federal tax mechanics — not personalized tax, legal, or financial
advice. Have a CPA, ERISA attorney, or fiduciary advisor review any real structure.
