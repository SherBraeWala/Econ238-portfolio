# Arjun Aujla - Econ238-portfolio

## Assignments
-Assignment 1 
---
layout: page
title: "What a Gallon Actually Tells You"
subtitle: "A one-page guide to reading data center headlines"
date: 2026-09-06
---

<!--
NOTE TO SELF — DELETE BEFORE PUBLISHING
Match the frontmatter fields above to whatever your other econ238-portfolio
pages use. If your existing pages use `layout: default` or a `permalink:`
field, copy that exactly — mismatched frontmatter is the usual reason a
Jekyll page fails to render.
All tables and bar charts below are plain markdown/unicode and will render
anywhere. If your theme supports Mermaid, the optional diagram in Section 5
can be swapped in; if not, the table version is already there.
-->

# What a Gallon Actually Tells You

**A guide to reading the next data center headline you see.**

> NEW AI DATA CENTER WILL CONSUME 800,000 GALLONS OF WATER EVERY DAY

*[YOUR OPENING — 3–4 sentences. Concede the reader's reaction is reasonable; that
number sounds enormous and they are not stupid for reacting to it. Then state
your thesis in one line: the number is real, but by itself it tells you almost
nothing, and the things worth worrying about are hiding underneath it.]*

---

## 1. The same number, two institutions

Here is that headline figure next to something in the same city as most readers
of this page.

| | Daily water | Land | Buildings | Grid electricity |
|---|---|---|---|---|
| **Colossus I** (xAI, Memphis) | ~812,500 gal/day <br><sub>MLGW data, March 2026</sub> | 217 acres | 785,000 sq ft | 150 MW service |
| **University of Rochester / UR Medicine** | ~685,000 gal/day <br><sub>core campus, UR utilities guide</sub> | 700+ acres | 15M+ sq ft | ~225M kWh/yr |

Water use, per day, same order of magnitude:

```
Colossus I   ████████████████████████  812,500 gal
U of R       ████████████████████      685,000 gal
```

*[YOUR PARAGRAPH — the point is not "therefore data centers are fine." The point
is that a number capable of producing a protest at one address produces nothing
at the other. Ask why. This is where you introduce "as compared to what?" as the
reader's first tool.]*

---

## 2. Withdrawal is not consumption

The single most useful distinction on this page.

| Term | What it means | Does the water come back? |
|---|---|---|
| **Withdrawal** | Water taken in | Usually most of it |
| **Consumption** | Water evaporated or otherwise not returned | No |
| **Discharge permit** | The legal *maximum* allowed | Not a measure of use at all |

The University reports roughly 250 million gallons of domestic water a year and
roughly 250 million gallons of sanitary flow a year. Those are largely the same
water, measured on the way in and on the way out. Adding them into "half a
billion gallons" would describe a quantity nobody used.

The University also holds a permit allowing discharge of up to 45 million gallons
a day of non-contact cooling water into the Genesee River. A ceiling on returning
water is not a measure of drinking water consumed.

**Cooling design decides how much is truly consumed:**

| Cooling type | Water consumed | Electricity used |
|---|---|---|
| Evaporative | High | Lower |
| Closed-loop / dry | Very low | Higher |

*[YOUR PARAGRAPH — draw the trade explicitly: water and power are substitutes in
cooling, so "uses less water" and "uses less electricity" are usually not the
same facility. A reader who takes away only this section has still gained
something real.]*

---

## 3. Making the numbers legible

Back-of-envelope, assumptions stated: 300 gallons/day per US household, 10,500
kWh/year per US household.

| Raw figure | In household terms |
|---|---|
| 812,500 gal/day | ≈ 2,700 households |
| 685,000 gal/day (U of R) | ≈ 2,300 households |
| 1.31 billion kWh/yr (150 MW run continuously) | ≈ 125,000 households |
| 225 million kWh/yr (U of R) | ≈ 21,000 households |

*[YOUR PARAGRAPH — note what this does to each headline. "As much water as a
city" collapses to a neighborhood. "As much electricity as a city" survives the
translation much better. One scary number shrinks under scrutiny and one does
not, and telling the reader *which* is the whole service you are providing.]*

---

## 4. Now the part that deserves the alarm

*[SECTION INTRO — one line signalling the turn: you have spent three sections
lowering the temperature, and you are about to raise it.]*

**Water.** *[Your paragraph: municipal water is typically priced at the cost of
delivering it, not at its scarcity value. A large buyer can pay every bill in
full and still leave a stressed aquifer worse off. This is a pricing failure, not
a volume problem — which means the remedy is a price, not a ban.]*

**The marginal kilowatt-hour.** *[Your paragraph: adding load to a grid where gas
sets the margin means the additional electricity is fossil-generated regardless
of what clean-power contracts the company has signed. Green procurement and
marginal emissions are different things.]*

**Who pays for the wires.** *[Your paragraph: new substations and transmission
get paid for by somebody. Whether that is the company or every ratepayer in the
region is a distributional choice made by a public utility commission, not a
technical fact. In Memphis, MLGW reported the transmission work was to be built
at xAI's expense — that is the kind of term residents should be reading.]*

---

## 5. What happens if we say no

Restricting a facility does not delete the demand for it. It relocates it.

| Policy | First-order effect | What comes next |
|---|---|---|
| Moratorium (NY, July 2026) | No local construction | Demand moves to a state with a dirtier grid and weaker review |
| Site far from population | Fewer neighbors affected | Thin transmission → on-site generation. Colossus 2 relied on 59 gas turbines, mostly across the Mississippi line (Reuters, July 2026), with a nitrogen-oxides dispute attached |
| Charge scarcity prices for water and grid capacity | Higher cost to operator | Closed-loop cooling and off-peak operation become worth paying for |

*[YOUR PARAGRAPH — this is your Nth-order consequence and the professor asks for
at least one. Emphasize that the turbine outcome is what "move it away from
people" can actually produce: more combustion, next to fewer and poorer people
with less capacity to object. Do not present this as an argument against
restriction. Present it as the cost of restriction, which has to be weighed
against its benefit.]*

---

## 6. Three questions to ask instead

*[Rewrite these in your own words once the piece is drafted — they should follow
from your sections, not sit on top of them.]*

1. **Is that withdrawal or consumption**, and what is the cooling design?
2. **Who pays for the new grid infrastructure** — the company or the ratepayers?
3. **Does the price of water and power here reflect scarcity**, or the cost of delivery?

*[CLOSING — 2–3 sentences. The reader should leave with a tool, not a verdict.]*

---

## Sources

- University of Rochester, Administration and Finance — utilities and facilities reporting
- University of Rochester 2024 waste report
- NYS Department of Environmental Conservation — SPDES discharge permit
- Memphis Light, Gas & Water — Colossus I electrical service and recycled water facility
- *Memphis Flyer* — March 2026 water purchase figures
- Reuters, July 2026 — Colossus 2 turbine investigation
- PR Newswire — Colossus I site description
- Office of Governor Kathy Hochul — July 2026 hyperscale data center moratorium
- EPA WaterSense and EIA — household water and electricity averages used in Section 3

<sub>Written for Econ 238, University of Rochester. All figures linked to public
sources; back-of-envelope calculations state their assumptions.</sub>
