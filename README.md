# Arjun Aujla - Econ238-portfolio

## Assignments
-Assignment 1 
---
layout: page
title: "What a Gallon Actually Tells You"
subtitle: "A one-page guide to reading data center headlines"
date: 2026-09-06
---

# What a Gallon Actually Tells You

**A guide to reading the next data center headline you see.**

> NEW AI DATA CENTER WILL CONSUME 800,000 GALLONS OF WATER EVERY DAY

Eight hundred thousand gallons a day is a lot of water. If that headline made you
uneasy, you were not being unreasonable. But a number that large is only the
beginning of a question, not the end of one, and the honest answer to "should I
be worried about this?" turns out to depend on things the headline never
mentions: whether the water comes back, what the facility is cooled with, who
pays for the power lines, and how many more of these get built. This page is
about how to ask those questions.

---

## 1. The same number, two institutions

Here is that headline figure next to an institution most people in Rochester
walk past without alarm.

| | Daily water | Land | Buildings | Grid electricity |
|---|---|---|---|---|
| **Colossus I** (xAI, Memphis) | ~812,500 gal/day <br><sub>MLGW data, March 2026</sub> | 217 acres | 785,000 sq ft | 150 MW service |
| **University of Rochester / UR Medicine** | ~685,000 gal/day <br><sub>core campus, UR utilities guide</sub> | 700+ acres | 15M+ sq ft | ~225M kWh/yr |

```
Colossus I   ████████████████████████  812,500 gal/day
U of R       ████████████████████      685,000 gal/day
```

These are the same order of magnitude. A hospital system and university that
nobody protests uses nearly as much water every day as the AI facility that
generated national coverage.

That comparison is not an argument that data centers are harmless. It is an
argument that the number by itself was never doing the work we thought it was
doing. Large institutions use large amounts of water. We already live alongside
infrastructure at this scale and mostly do not notice it. So when a figure
provokes outrage at one address and indifference at another, something other
than the figure is driving the reaction, and it is worth knowing what.

The real question is not whether *this* facility uses a lot. It is what happens
when we add many of them.

---

## 2. Withdrawal is not consumption

This is the most useful distinction on the page, and almost no headline makes it.

| Term | What it means | Does the water come back? |
|---|---|---|
| **Withdrawal** | Water taken in | Usually most of it |
| **Consumption** | Water evaporated or otherwise not returned | No |
| **Discharge permit** | The legal *maximum* allowed | Not a measure of use at all |

The University reports roughly 250 million gallons of domestic water a year and
roughly 250 million gallons of sanitary flow a year. Those are largely the same
water, counted on the way in and again on the way out. Adding them together to
get half a billion gallons would describe a quantity that no one ever used. The
University also holds a permit allowing discharge of up to 45 million gallons a
day of non-contact cooling water into the Genesee River — a ceiling on water
being *returned*, not drinking water consumed.

Water that is withdrawn, used, and returned is a fundamentally different thing
from water that is evaporated and gone. Which one a facility does is determined
by how it is cooled:

| Cooling type | Water consumed | Electricity used |
|---|---|---|
| Evaporative | High | Lower |
| Closed-loop / dry | Very low | Higher |

There is no design that minimizes both. Water and electricity are substitutes in
cooling, so a facility that solves its water problem has made its power problem
worse, and vice versa. Anyone promising you a data center that is easy on both is
selling something.

This also means "how much water does it use?" is the wrong question. "How much
does it consume, and what did it burn to consume less?" is the right one.

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

Watch what translation does. "As much water as a small city" becomes about 2,700
households — a neighborhood, in a metro area with something like a quarter of a
million of them. That headline shrinks badly under scrutiny.

The electricity headline does not. A 150 MW load running continuously is on the
order of 125,000 households of demand, and Colossus I has another 150 MW
increment planned. That one survives translation, and it is the number that
should hold your attention.

So of the two scary figures in the news, one mostly dissolves and one gets worse
the closer you look. Knowing which is which is the entire service this page is
trying to provide.

And here is where the aggregate matters. One facility drawing a neighborhood's
worth of water is unremarkable. A hundred of them, sited in the same handful of
regions with cheap land and cheap power, is a different proposition entirely.
Almost nobody is modeling that cumulative path, and the absence of that modeling
is a better reason for concern than any single project's permit.

---

## 4. Now the part that deserves the alarm

Three things underneath the headlines are genuine problems. None of them is
"large volume."

**Freshwater is the wrong input.** The objection worth making is not that data
centers use water, but that they use *drinking* water — treated to a standard no
cooling tower requires, drawn from aquifers and municipal systems that
communities depend on. The alternative is not exotic. In Memphis, MLGW has
described a recycled-wastewater facility designed to produce up to 13 million
gallons a day of reclaimed industrial water, with xAI stating it intends to spend
more than $80 million toward it. That is the shape of a real answer: reclaimed
water, closed loops, non-potable sources. Whether it gets built on time is a
separate and contested question — but it demonstrates that the water problem is
an engineering and financing problem, not a law of nature.

**The marginal kilowatt-hour is dirtier than the contract says.** Adding a large
load to a grid where natural gas sets the margin means the additional electricity
is gas-fired, whatever clean-power agreements the company has signed. This is why
the water fix and the carbon fix pull against each other: closed-loop cooling
saves water by demanding more power from exactly that margin. Pairing facilities
with dedicated renewable generation helps, but a data center runs around the
clock and solar does not, so without serious storage the grid still fills the
gap. The cleaner the local grid, the better every one of these trades gets — which
makes grid decarbonization the highest-leverage policy here, and it has nothing
to do with data centers specifically.

**Somebody pays for the wires.** New substations and transmission are expensive,
and whether that cost lands on the company or on every ratepayer in the region is
a decision made by a utility commission, not a fact of engineering. It should
land on the firm. A private company building a private facility for private
profit can finance its own infrastructure, through debt or equity, and in Memphis
MLGW reported that the transmission improvements and new substation were to be
built at xAI's expense. That is the term residents should be reading for, and its
absence is the clearest signal that a deal is bad for the community.

One consequence follows and should be said plainly: as demand rises against a
supply of water and generating capacity that expands only slowly, prices go up.
That is not the harm. That is the mechanism. A price that reflects scarcity is
what makes reclaimed water, closed loops, and off-peak operation worth paying
for. A price that reflects only the cost of delivery guarantees that nobody
bothers.

---

## 5. What happens if we say no

Refusing a facility does not delete the demand for it. It moves it.

| Policy | First-order effect | What comes next |
|---|---|---|
| Moratorium (NY, July 2026) | No local construction | Demand shifts to states with dirtier grids and weaker review |
| Site far from population | Fewer neighbors affected | Thin transmission → on-site generation. Colossus 2 relied on 59 turbines, mostly across the Mississippi state line (Reuters, July 2026), with a nitrogen-oxides dispute attached |
| Price water and grid capacity at scarcity | Higher operating cost | Closed-loop cooling, reclaimed water, and off-peak operation become worth the investment |

The middle row deserves attention because it is the intuitive policy. Put them
where nobody lives. But empty places have empty grids, and a facility that cannot
get transmission generates its own power on site. "Move it away from people" can
therefore produce *more* combustion, next to fewer and poorer people with less
capacity to object. That is not an argument against restriction. It is the cost
of restriction, and it has to be weighed rather than assumed away.

There is a larger version of the same logic. Compute capacity is the
infrastructure the next several decades of economic activity will be built on. A
region that blocks all of it does not avoid the tradeoff; it exports the
investment and keeps the disadvantage. That is a real consideration. It is not,
however, a blank check — "we will fall behind" is an argument for building
capacity somewhere, not an argument against making anyone pay for their own
substation.

The version that survives scrutiny: restriction and encouragement are both
choices with consequences, and the third row of that table is the one that
actually changes behavior instead of relocating it.

---

## 6. Three questions to ask instead

The next time a project is proposed near you, these will tell you more than any
headline figure:

1. **Is that withdrawal or consumption** — and is the facility cooled with
   drinking water, reclaimed water, or a closed loop?
2. **Who is paying for the new substations and transmission** — the company, or
   every ratepayer in the region?
3. **Does the price of water and power here reflect scarcity**, or only the cost
   of delivery?

None of these produces a verdict. Together they produce something better: the
ability to tell the difference between a project that imposes real costs on
people who never agreed to bear them, and a project that is simply large.

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

<sub>Written for Econ 238, University of Rochester. Back-of-envelope calculations
state their assumptions.</sub>
