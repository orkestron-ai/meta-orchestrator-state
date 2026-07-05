# Leadership Selection & Succession — power that changes hands without rupture

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Fills** | gap **G2** (leadership selection, succession, peaceful transfer of power) |
| **Grounds** | orkestro.net Position / **PositionMemory (BR8)** / Assignment / TrackRecord / ControlPolicy; Charter supremacy; Principle 10 (decay) |
| **Created** | 2026-06-28 |

> A state that cannot **select, rotate, hold accountable, remove, and peacefully transfer**
> its offices is not a state — this is democracy's crown jewel, and it was our biggest gap.
> Axiacracy's answer leverages what it uniquely has: **offices whose memory outlives their
> holders, continuous performance accountability, and sovereignty vested in the Charter, not
> in a person.**

## 1. Separation of powers, Axiacracy-style

| Branch | Who | Function |
|---|---|---|
| **Legislative** | the **demos** — citizen weight-voting + party delegation | sets **values**: axis weights, floor thresholds, mandates |
| **Executive** | the **Sub-Agents** (each owns one axis) + a coordinating role | **pursue** the mandates within corridors |
| **Judicial** | courts + constitutional review + Equity/Ombudsman guardian | **review** Charter-conformance, adjudicate, protect floors |

*Citizens legislate values; Sub-Agents execute; courts review.* The Charter is above all three.

## 2. Selection — "vote on values, appoint on competence"

Pure election of a *technical* office (balance a value dimension) invites populism; pure
meritocracy invites technocratic capture. The synthesis:

- The **mandate** (what to optimize = weights + floors) is **democratic** (voted).
- The **filling of the Position** is **competence-based** — the best-**calibrated** agent in
  that domain is **assigned** (orkestro.net Assignment; TrackRecord/Brier-calibration).
- The assignment is **revocable on performance.**

→ **Citizens set the goal (democratic); the most competent agent is assigned to pursue it
(meritocratic); the seat is performance-revocable.** This mirrors the values/execution split
(cf. futarchy's values/beliefs) and dodges both populism and technocracy. **Sortition** (random
selection) is reserved for **oversight/jury bodies** (citizen review panels, constitutional
juries) as an anti-capture counterweight.

## 3. Tenure, rotation & institutional memory

- **Bounded terms + mandatory rotation** (anti-entrenchment; Principle 10).
- **PositionMemory outlives the holder (BR8).** Institutional knowledge belongs to the
  **office**, not the agent — so you can **rotate the officeholder without losing
  institutional memory**. Real states hemorrhage knowledge at every turnover; Axiacracy does
  not. **Continuity of the office is decoupled from continuity of the officeholder.**
- **Autonomy ramps with TrackRecord but is capped and decays** on poor performance or rising
  concentration — even a good officeholder cannot entrench.

## 4. Accountability & removal — continuous, not just periodic

- A Sub-Agent's **KPI is measured continuously (E3)**: how well its dimension is balanced and
  growing **without raising anti-value, without pushing a cohort below floor, without
  breaking participation conditions**. Poor performance → autonomy tightening → removal.
  **Continuous accountability** beats waiting for the next election.
- **Recall / impeachment:** citizens, the judiciary, or the guardian can trigger review of an
  organ; the **same courts + constitutional-review** machinery adjudicates.
- **Capture / concealment → clawback + removal** — the anti-value machinery applies to state
  organs too (Principle 10, explicitly not just to citizens/BigTech).

## 5. Peaceful transfer of power — the hard problem, structurally defused

Transfers fail in reality because power is **lumpy** (one office holds everything) and the
loser loses everything. Axiacracy removes those conditions:

- **Power is distributed and continuous, not a throne.** Sovereignty is in the **Charter**;
  Sub-Agents each hold **one axis**; the demos and courts hold the rest. **There is no single
  seat to seize** — the federation-of-frames structure divides power by construction.
- **Transfer is gradual, not binary.** Authority flows via TrackRecord/autonomy ramps, not a
  winner-take-all election-night flip — the losing holder does not lose *everything at once*,
  cutting the incentive to refuse.
- **Transparency voids seizure.** All agent logic and rulings are on the verifiable log; an
  organ ignoring a legitimate removal is **immediately visible and Charter-void (Art. 20)** —
  its subsequent acts are **void**, so seizing office yields **nothing legitimate**.
- **Loyalty is to the Charter, not the person.** The coercive/administrative apparatus draws
  its legitimacy (and its agents' standing) from **Charter-conformance**; obeying an
  unconstitutional seizure is itself a Charter breach that **voids the actors' standing**
  (the structural bulwark; deepened in gap **G3 — defense/monopoly on force**, next phase).
- **No vacuum on turnover.** PositionMemory carries the office across the handover — continuity
  without rupture.

## 5a. What succession actually is — hot-swapping the algorithmic officeholder, and candidate validation

Precisely: an Axiacratic "transfer of power" is **replacing the agent implementation (vendor
or major version) that fills a Position — not changing the form of government.** The
**Charter/regime is stable**; only the *officeholder's implementation* rotates. Two invariants
make it safe:

- **PositionMemory persists** across the swap (institutional continuity, §3).
- **The officeholder's code is open and verifiable** — the *decision logic and algorithms of
  officials are public and auditable*, a first-class Axiacracy transparency principle (Charter
  Art. 16). Decisions cite the **logic-hash** that produced them; a **reproducible build**
  proves the running agent *is* the audited code.

**Candidate validation (the vetting gate).** Before an agent may fill a Position it must pass
validation against: **system abuse** (metric-gaming / Goodhart); **regime-change attempts**
(anything eroding the Charter, esp. the eternity core); and **hidden value-redirection** —
covert, clever, multi-step diversion of the primary value flows to hidden beneficiaries.

Mechanisms:
- **Reproducible build + logic-hash** — running logic must match the audited public code (supply-chain integrity).
- **Adversarial red-team before assignment** — alignment/security evals hunting metric-gaming, Charter-violating paths, and covert diversion.
- **Flow-conservation & beneficiary audits — the structural defense.** Because **all value
  moves as visible flows (VMT A3)**, a hidden diversion *must surface as a flow* — and as
  **unearned capture (= rent, `Property-Rent-and-Commons.md`)** toward some beneficiary. **You
  cannot secretly redirect value in a system where all value moves as visible, ledgered flows.**
  The same transparency that audits decisions makes hidden beneficiaries detectable as
  flow/rent anomalies.
- **Multi-vendor diversity** — no single vendor fills all Positions (supply-chain concentration
  = anti-value); independent implementations **cross-check** each other — a decision diverging
  from what an independent agent would decide flags manipulation (requisite variety, gap G8).
- **Staged autonomy on version change** — a new vendor/major-version starts under tight
  ControlPolicy checkpoints (low autonomy, high review) and **earns** autonomy via TrackRecord;
  the blast radius of a bad/compromised version is bounded.
- **Continuous monitoring + retrospective clawback** — vetting is ongoing; a **sleeper
  mechanism** that activates later is caught by monitoring and falls in the **concealment /
  perpetual-liability class** (clawback + removal, `Value-Money-Coupling.md` §4).

So Axiacratic succession is a **secure hot-swap of an open, validated algorithmic officeholder
over a persistent institutional memory** — the regime never changes; only vetted implementations do.

## 6. The coordinating role — Meta-Orchestrator as coordinator, not sovereign

Cross-axis conflicts (one Sub-Agent's action harming another's axis) need coordination — but
**not a ruler**. The **Meta-Orchestrator** is a **coordinating Position**: it **resolves
cross-axis conflict within the Charter**, is **rotating, Charter-bound, performance-revocable,
and holds no unchecked authority**. It **coordinates, it does not rule** — consistent with
"the state is a router, not an apex." (The doctrine's very name denotes coordination, not
sovereignty.)

## 7. Guarding the guardians (overlapping, polycentric)

No single organ is unchecked: (i) the **democratic mandate** constrains each Sub-Agent's
goal; (ii) **courts + constitutional review** check Charter-conformance; (iii) the
**Equity/Ombudsman** guardian checks distributional fairness; (iv) **cross-axis anti-value** —
harming another axis is visible and charged; (v) **TrackRecord/autonomy decay**; (vi)
**citizen recall + sortition juries**. Multiple overlapping checks (Ostrom polycentricity).

## Registry / Charter notes (batch later)
- Extend **A2 Branch of Power** with `selection(mandate-democratic/assignment-competence)`,
  `term`, `rotation`, `recall`, `transfer`.
- New/explicit **A10 Coordinating Role (Meta-Orchestrator)** — rotating, Charter-bound coordinator.
- Possible Charter article (Part VI): *"Sovereignty vests in the Charter, not in any office;
  offices are competence-assigned under a democratic mandate, rotating, performance-revocable;
  loyalty of all organs runs to the Charter."*

## Open knobs for the owner
- Term length / rotation cadence; how much autonomy a proven officeholder may accrue before the cap.
- Is there a single coordinating Meta-Orchestrator, or a rotating **council** of Sub-Agents?
- Sortition scope: which oversight bodies are randomly selected vs competence-assigned.
- P0: do we model organ selection/rotation at all, or fix the Sub-Agents for the first loop?
