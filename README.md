# Water Treatment Field Calculator

A single-file, fully offline calculator suite for industrial water treatment field reps.

**→ Open `water-treatment-calculator.html` in any modern browser. That's it — no install, no internet, no server.**

## What's inside

**70 calculators** across six modules, each returning numbers **plus a plain-language verdict, warning flags, and an expandable "show your work" panel** with the substituted formula:

| Module | Coverage |
|---|---|
| **Pretreatment** (PT-01…16) | Hardness conversions, compensated hardness, softener sizing/geometry/brine/audit, leakage estimator, chloride & split-stream & WAC dealkalization, decarbonators, filter sizing, carbon EBCT, SMBS dechlorination, Fe/Mn oxidation |
| **Boilers** (BL-01…16) | Cycles by tracer, blowdown & water balance, steam load 3 ways, ASME/ABMA max-cycles limit finder, blowdown savings ($), heat recovery, condensate return value, feedwater blend, O₂ scavengers, DA performance, internal treatment, P/M/OH alkalinity, carryover, amine demand, softener-failure impact |
| **Cooling Towers** (CT-01…15) | Range/approach/efficiency, heat load, water balance, measured & reconciled COC, max safe cycles, LSI (bulk + skin), LSI/RSI/PSI/Larson-Skold dashboard with cycle projector, system volume & holding time, inhibitor feed, biocide slug/oxidizing dosing, acid feed, corrosion coupons |
| **Reverse Osmosis** (RO-01…11) | Recovery/rejection/CF, flux, osmotic & net driving pressure, ASTM normalization, 10-15-15 cleaning triggers with foulant diagnosis, concentrate scaling + max safe recovery, antiscalant/acid dosing, permeate projection, SDI, array staging check, CIP |
| **Closed Loops** (CL-01…09) | System volume (tracer/takeoff/rules), heat load & low-ΔT diagnostic, glycol freeze/burst/derate/blending, inhibitor dosing, leak detection from inhibitor decay, loop water quality assessment, flush & passivation |
| **Utilities** (CU-01…06) | Universal chemical feed + drawdown stopwatch, dilution, ROI builder, titration helper, ion ⇄ CaCO₃ converter, conductivity ⇄ TDS |

Plus a browsable **Reference** section (ASME/ABMA limits, steam tables, glycol tables, pipe volumes, resin capacities, chemical densities, and more) and a **Settings** page where every house constant and limit is editable.

## Key features

- **Shared water analysis** — organized around the tests reps actually run (hardness, iron, free/total chlorine, phosphate, copper, sulfite, chloride, nitrate, molybdate, condensate pH…); any input with a "⇩ analysis" chip pulls from it
- **Biocide quarter-life dosing** — CT-13 gives both the dilution-model quarter-life and the house estimating formula ln(¼)/(1−1/(COC−1))
- **Live validation** — amber for unusual values, red block for physically impossible ones
- **Charts** — savings breakdowns, blowdown-vs-cycles curves, glycol curves, TCF, index gauges, decay curves (all inline SVG, theme-aware, with hover tooltips)
- **Everything persists** in the browser (localStorage): inputs, water analysis, settings, theme
- **Metric toggle** shows metric equivalents beside results (internal math stays in US units, 8.34 lb/gal basis)
- **Copy results / Print** for customer-facing summaries with the assumptions visible
- Light/dark theme, phone-friendly layout, search by ID or name

## Disclaimer

Results are engineering estimates for field guidance. Boiler and pressure-vessel water chemistry must comply with the manufacturer's requirements, jurisdictional code, and the site's insurer. ASME/ABMA values are *suggested consensus limits*, not code. Legionella control requires a formal water management plan (ASHRAE 188) — a biocide calculation is not a control program. Lookup values (resin capacities, leakage factors, inhibitor ranges) are typical published defaults; tune them in Settings to your house program and product data sheets.
