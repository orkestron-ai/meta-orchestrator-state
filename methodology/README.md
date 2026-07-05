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
| **[`Axiacracy-Compendium.md`](./Axiacracy-Compendium.md)** | **★★ START HERE — single-source overview of the whole doctrine** (synthesizes every doc + the Charter + the registry, end to end) |
| **[`Charter.md`](./Charter.md)** | **★ The supreme document (meta-constitution, jus cogens).** 22 articles in 6 parts — the value-balancing mandate, inviolable rights & per-cohort floors, governance principles, money/markets, epistemic & judicial integrity, supremacy & eternity clause. Everything else elaborates it |
| [`Governance-Mechanics.md`](./Governance-Mechanics.md) | **Core rationale.** Principles A0 (15, the annotated source of the Charter articles), organizational mechanics B0 (minority protection, parties = liquid democracy, experts/anti-propaganda, peer recognition), communication & transparency C0 |
| [`Value-Axes-Corridors-Voting.md`](./Value-Axes-Corridors-Voting.md) | The 10 value axes, per-cohort/region corridors, quadratic weight voting + delegation, the imbalance signal (floor/equity penalties not weight-scaled) |
| [`Consumption-and-Settlement.md`](./Consumption-and-Settlement.md) | How citizens spend earned value; two-layer (sovereign ledger + thin settlement rail); proportional ceremony; default-trust reclamations |
| [`Markets-and-Civilizational-Value.md`](./Markets-and-Civilizational-Value.md) | Reconciling revealed (market) vs deliberative (state) value; the market clears, the state prices the externality residual; profit decoupled from civ-value |
| [`Value-Money-Coupling.md`](./Value-Money-Coupling.md) | Instant enforcement (escrow, continuous anti-value debit, concentration charge, standing loss) + retrospective clawback; finality for the honest, perpetual liability for the concealing |
| [`Courts-and-Adjudication.md`](./Courts-and-Adjudication.md) | Anti-value is interpretable but contestable; courts judge by **contemporaneous norms**; versioned norm-set; non-retroactivity |
| [`Value-Frames-and-Perspectival-Value.md`](./Value-Frames-and-Perspectival-Value.md) | **VMT grounding.** Value is perspectival; MOS = a **federation of value systems** (frames), not one ledger; no state apex (forbidden by T1/A12/A10); participation condition θ; terminology aligned to VMT canon |
| [`Anti-Value-Taxonomy.md`](./Anti-Value-Taxonomy.md) | Anti-value classified by **scope** (edge/systemic), **detection lag** (→ enforcement instrument), and **type**; responsibility share (Shapley-style attribution); three worked profiles (yogurt / content-dependency / BigTech) through Planned→Realized→Retrospective |
| [`Relative-Value-and-Inter-Frame-Routing.md`](./Relative-Value-and-Inter-Frame-Routing.md) | No universal unit — **Realized Æ is the cross-currency invariant** (not price); intra-axis ratios = market discovery, inter-axis = voted weights; fairness is a constraint, not the objective. Measuring other frames lets the state **incentivize in the actor's own currency**, monitor θ, and **route positive-sum flows markets miss**. Part 3: **privacy-preserving frame disclosure** (scoped access → frame summary, not raw ledger) |
| [`Charter-Norm-Hierarchy-and-Rights.md`](./Charter-Norm-Hierarchy-and-Rights.md) | The **Axiacracy Charter** = a meta-constitution (jus cogens) **above** every polity's constitution & codes (conform-or-void; eternity clause). **Ultra-anti-value split by KIND**: rights-violation (not priced → criminal law) vs malicious vs distress (care) vs negligent. Incapacitation justified by protecting others' participation conditions (A9), not retribution. Subsidiarity of enforcement |
| [`Leadership-Selection-and-Succession.md`](./Leadership-Selection-and-Succession.md) | **Gap G2.** Separation of powers (demos legislates values / Sub-Agents execute / courts review); **vote on values, appoint on competence**; rotation **without losing PositionMemory**; continuous performance accountability; **peaceful transfer** structurally defused (power distributed not lumpy, transparency voids seizure, loyalty to the Charter not the person); Meta-Orchestrator = coordinator, not sovereign |
| [`Distributive-Justice-and-Capability-Floors.md`](./Distributive-Justice-and-Capability-Floors.md) | **Gap G6.** Axiacracy's justice stance: **capability sufficientarianism + bounded contribution-responsive band + anti-concentration ceiling + generosity premium** = the corridor, grounded. Floors in **capability-space** (Sen) not resources; realized Æ ≈ achieved functioning; Nussbaum's 10 → axis/rights crosswalk |
| [`Property-Rent-and-Commons.md`](./Property-Rent-and-Commons.md) | **Gap G1.** Own the earned, not the unearned: private ownership bounded by creation; **unearned rent (measurable as captured−created, VMT T11) is commons-owed**; **AI-compute/data = the new "land"** → rent to a citizen dividend + civilizational reinvestment; capital/credit/investment when money is demoted (returns to creation, not ownership) |
| [`Comparative-Analysis-and-Gaps.md`](./Comparative-Analysis-and-Gaps.md) | Coverage of Axiacracy vs rival orders (democracy, capitalism, socialism, Georgism, futarchy, doughnut economics, capability approach, Beer's VSM). Matrix + prioritized **gap backlog** (property/rent, succession, external relations, policy-efficacy, capability-grounded floors, …) |
| [`meta-models.csv`](./meta-models.csv) | Machine-readable registry of the **38 meta-models** (the semantic model of the state), synced to the methodology: adds V5 Value System/Frame, A0 Charter, A9 Rights, B7 Party/Delegation, B8 Expert, B9 Recognition, C5 Settlement/Escrow/Clawback, C6 Inter-Frame Routing |

All documents are **DRAFT, under discussion** — not yet ratified.
