# Methodology — the transferable value-flow governance blueprint

This directory is the **deployment-agnostic methodology** of the Meta-Orchestrator State:
the model of how a polity is governed by **balancing multidimensional value flows** instead
of taxation. It is written to be reusable **beyond the simulation** — a real government
could adopt it to build a MOS on entirely different infrastructure, with **human citizens
instead of AI agents**. (The simulation that *realizes* it on the Orkestron stack lives in
[`../implementation`](../implementation).)

> Relationship to the ecosystem: this methodology is to a *real state* what AISMM is to a
> *software product* — a meta-model/standard, not one implementation of it.

## What belongs here (methodology) vs. there (implementation)

| Methodology (here) | Implementation (`../implementation`) |
|---|---|
| value substrate (Value Transformer, Æ-vector, Value Flow, Anti-Value) as a **standard** | mapping to orkestro.net Personas/Positions |
| governance principles, corridors, liquid-democracy voting & parties | tiered cognitive fidelity, sim-clock, event ticks |
| markets ↔ civilizational value (Pigou overlay) | compute exchange, LLM-gateway, Go/n8n/Vault stack |
| value ↔ money coupling, escrow, clawback | the ~100-citizen P0 experiment runtime |
| courts, non-retroactivity, interpretation | hosting / scaling / federation deployment |
| the meta-model registry (the semantic model of the state) | — |

## Documents

| File | What it holds |
|------|---------------|
| [`Governance-Mechanics.md`](./Governance-Mechanics.md) | **Core.** Principles A0 (15), organizational mechanics B0 (minority protection, parties = liquid democracy, experts/anti-propaganda, peer recognition), communication & transparency C0 |
| [`Value-Axes-Corridors-Voting.md`](./Value-Axes-Corridors-Voting.md) | The 10 value axes, per-cohort/region corridors, quadratic weight voting + delegation, the imbalance signal (floor/equity penalties not weight-scaled) |
| [`Consumption-and-Settlement.md`](./Consumption-and-Settlement.md) | How citizens spend earned value; two-layer (sovereign ledger + thin settlement rail); proportional ceremony; default-trust reclamations |
| [`Markets-and-Civilizational-Value.md`](./Markets-and-Civilizational-Value.md) | Reconciling revealed (market) vs deliberative (state) value; the market clears, the state prices the externality residual; profit decoupled from civ-value |
| [`Value-Money-Coupling.md`](./Value-Money-Coupling.md) | Instant enforcement (escrow, continuous anti-value debit, concentration charge, standing loss) + retrospective clawback; finality for the honest, perpetual liability for the concealing |
| [`Courts-and-Adjudication.md`](./Courts-and-Adjudication.md) | Anti-value is interpretable but contestable; courts judge by **contemporaneous norms**; versioned norm-set; non-retroactivity |
| [`Value-Frames-and-Perspectival-Value.md`](./Value-Frames-and-Perspectival-Value.md) | **VMT grounding.** Value is perspectival; MOS = a **federation of value systems** (frames), not one ledger; no state apex (forbidden by T1/A12/A10); participation condition θ; terminology aligned to VMT canon |
| [`Anti-Value-Taxonomy.md`](./Anti-Value-Taxonomy.md) | Anti-value classified by **scope** (edge/systemic), **detection lag** (→ enforcement instrument), and **type**; responsibility share (Shapley-style attribution); three worked profiles (yogurt / content-dependency / BigTech) through Planned→Realized→Retrospective |
| [`Relative-Value-and-Inter-Frame-Routing.md`](./Relative-Value-and-Inter-Frame-Routing.md) | No universal unit — **Realized Æ is the cross-currency invariant** (not price); intra-axis ratios = market discovery, inter-axis = voted weights; fairness is a constraint, not the objective. Measuring other frames lets the state **incentivize in the actor's own currency**, monitor θ, and **route positive-sum flows markets miss**. Part 3: **privacy-preserving frame disclosure** (scoped access → frame summary, not raw ledger) |
| [`Charter-Norm-Hierarchy-and-Rights.md`](./Charter-Norm-Hierarchy-and-Rights.md) | The **Axiacracy Charter** = a meta-constitution (jus cogens) **above** every polity's constitution & codes (conform-or-void; eternity clause). **Ultra-anti-value split by KIND**: rights-violation (not priced → criminal law) vs malicious vs distress (care) vs negligent. Incapacitation justified by protecting others' participation conditions (A9), not retribution. Subsidiarity of enforcement |
| [`meta-models.csv`](./meta-models.csv) | Machine-readable registry of the ~30 meta-models (the semantic model of the state) |

All documents are **DRAFT, under discussion** — not yet ratified.
