# Anti-Value Taxonomy — scope, attribution, lag, and lifecycle

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Completes** | the V4 Anti-Value methodology before P0 |
| **Grounds** | VMT A5 (anti-value independent), T4 (flow resistance accumulates), T6 (distortion reduces future capacity), A11 (leakage), A8/A9/T7 (participation condition) |
| **Created** | 2026-06-28 |

> How anti-value is **classified, measured, and attributed** — *before* it is charged (the
> charging mechanics live in `Value-Money-Coupling.md`). The taxonomy explains why one
> machine handles three very different harms (a spoiled yogurt, content dependency, BigTech
> concentration), and why both instant and retrospective enforcement are necessary.

## 0. Anti-value is independent, not "negative value" (A5)

A single flow can carry **+value AND +anti-value at once** (BigTech: real economic value
*and* real concentration harm). They are booked on **separate axes** and **not netted in
the ledger**. Net standing/civ-value is computed *for decisions*, but the ledger preserves
both — so a "high-value, high-anti-value" actor is **visible as such**, not blurred into a
mediocre middle.

## 1. Three classifying dimensions

| Dimension | Values | Determines |
|---|---|---|
| **Scope** | `edge` \| `systemic` | how it is attributed |
| **Detection lag** | `immediate` \| `short` \| `long` \| `generational` | which enforcement instrument applies |
| **Type** | (catalogue below) | which axis/cohort/Sub-Agent owns it |

## 2. Scope — edge vs systemic

- **Edge anti-value** — attributable to a **single value flow**. Booked on that flow.
  *Spoiled yogurt → this transaction harmed this citizen.* Attribution is trivial (one actor).
- **Systemic anti-value** — emerges from a **pattern over many flows**, **not reducible to
  any single flow** (no individual video addicts you; no single deal is a monopoly). Booked
  on the **pattern**, then **attributed back** via a responsibility share (§3).

> VMT grounding: systemic anti-value *is* accumulated **Flow Resistance** (T4) / **Leakage**
> (A11) at the system level, and it *reduces the system's future capacity to realize value*
> (T6). It is a property of the value system, not of an edge.

## 3. Attribution — the responsibility share (for systemic anti-value)

How to split blame across contributing flows/actors. A **published attribution function**:

1. **Default — marginal contribution (Shapley-style).** Each actor's share = its marginal
   contribution to the systemic harm, averaged over orderings. Fair under standard axioms;
   approximated cheaply in simulation (sampled orderings).
2. **Fallback — proportional exposure.** Share ∝ the actor's volume/intensity of the
   contributing flow type (e.g., share of total attention-hours captured). Cheap, used when
   marginal computation is infeasible.
3. **Threshold / dose handling.** Nonlinear harms (concentration): the actor that **crossed
   the threshold** bears the marginal charge (ties to the economic ceiling).
4. **Concealment multiplier.** An actor that **hid** its contribution or its flow resistance
   (T9 hidden flows, T17 interpretive distortion) bears a **higher share** → links to the
   perpetual-clawback class.

Responsibility shares are **Planned→Realized→Retrospective like any valuation**: provisional,
contestable in court, and **re-allocated as evidence accrues** — under **contemporaneous
norms** (the attribution-function version in force at act-time; `Courts-and-Adjudication.md`).

## 4. Detection lag → enforcement instrument

The latency between act and measurable harm decides *how* it bites:

| Lag | Example | Instrument (from `Value-Money-Coupling.md`) |
|---|---|---|
| **immediate** (≈0) | ecological emission, spoiled good detected at sale | continuous anti-value debit |
| **short** (days–weeks) | service failure, early dependency signal | **escrow** holds; reclamation window |
| **long** (months–years) | content dependency, cognitive degradation, concentration | **retrospective revaluation + clawback** (escrow can't hold that long) |
| **generational** (years–decades) | demographic decline, intergenerational meaning-loss | structural / Demography Sub-Agent as **trustee for future cohorts** |

**This is why both halves exist.** Escrow sizing should track the externality's lag; for
long/generational lag, escrow is structurally insufficient → retrospective clawback is
*required*, not optional.

## 5. Measurement — honest about the hard part

- **Edge:** the **realized-value gap** directly — `Planned − Realized` on the harmed axes,
  attested by the victim. Measurable.
- **Systemic:** the Sub-Agent measures the **dimension's decline across a cohort** and
  attributes the **excess over a baseline/counterfactual** to the contributing flow-pattern.
  Causal-inference-hard in reality. The magnitude is itself **interpretable, provisional,
  revaluable**, and the estimator is **calibration-scored** (Brier) like an expert.
- **Simulation advantage (P0):** we have **ground truth** for the systemic effect (computable
  from the model), so we can compare the state's **estimate** against the **true** anti-value
  and measure the state's **epistemic accuracy** — something reality can never do. A first-
  class P0 experiment.

## 6. Three worked profiles (Planned → Realized → Retrospective)

### (a) Spoiled yogurt — **edge**, short lag
- **Planned** (business): +nutrition; no anti-value intended.
- **Realized** (citizen): −health (poisoning); huge **Flow Resistance** (Planned ≫ Realized).
- **Retrospective**: if spoilage recurs across citizens → **escalates edge → systemic**
  (the business's quality leakage), re-priced.
- Attribution 100% the business · Instrument: reclamation + escrow forfeit.

### (b) Content dependency — **systemic**, long lag
- **Planned** (platform): +entertainment/economic; engagement claimed as value.
- **Realized** (citizen, per session): looks **neutral/mildly positive** — *the trap: no edge
  is harmful.*
- **Retrospective** (thousands of flows, months on): −cognitive, −meaning, dependency;
  emerges only at the **pattern** (T6). The **vote-vs-spend gap** is the early tell.
- Attribution: responsibility share across attention-capturing platforms (proportional +
  concealment multiplier if engagement-optimization was hidden) · Instrument: retrospective
  revaluation + clawback; **Cognitive Health Sub-Agent reshapes the demand field, does not ban.**

### (c) BigTech concentration — **systemic**, continuous + long lag
- **Planned** (firm): +economic, +infrastructural (genuinely productive — the article concedes this).
- **Realized** (customers): positive per deal (good product).
- **Retrospective/systemic**: value concentration → −economic opportunity, −social_stability,
  dependency, displacement; from **accumulation**, not any single deal. The article's central case.
- Attribution: the concentrating actor (it *is* the concentration) · Instrument: **BOTH** —
  continuous **concentration charge** (prevention, ceiling) **and** retrospective **clawback**
  if concealed/gross. Uses the full machinery.

These three span the space: edge/short · systemic/long · systemic/continuous+long.

## 7. V4 Anti-Value object fields
`type` · `scope` (edge|systemic) · `axis` (harmed Æ dimension) · `magnitude` (+ confidence) ·
`form` (Planned|Realized|Retrospective) · `lag` (immediate|short|long|generational) ·
`attributed_flows[]` · `responsibility_share[]` · `concealment` (degree → multiplier,
clawback eligibility) · `baseline` (counterfactual for excess) · `estimator_version`
(commit-hash → reproducibility + non-retroactivity).

## 8. Link to participation conditions
Systemic anti-value that pushes a **cohort's participation condition θ below threshold**
(A8/A9/T7) is the **highest-priority alarm** — it threatens the sustainability of the state's
own value system (`Value-Frames-and-Perspectival-Value.md` §3). It outranks ordinary
imbalance.

## Open knobs for the owner
- Shapley-approximation budget (sampled orderings) vs proportional-only for P0.
- Baseline/counterfactual definition for systemic measurement (rolling vs constitutional).
- Lag thresholds per axis; escrow hold-period as a function of lag.
- The concealment test (what counts as "hidden") — shared with the clawback-eligibility test.
