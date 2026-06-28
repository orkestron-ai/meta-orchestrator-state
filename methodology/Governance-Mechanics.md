# Governance Mechanics — Meta-Orchestrator State

| | |
|---|---|
| **Status** | **DRAFT v0.2 — under discussion, not yet ratified** |
| **Author** | Victor Bolshakov (design dialogue) |
| **Supersedes** | §11 open questions in `Meta-Orchestrator-State-Project.md` (partially) |
| **Created** | 2026-06-28 |

> This document captures the **governance layer** of MOS — how the value-flow-governed
> state is actually *run by its citizens*: principles (A0), organizational mechanics
> (B0: parties, experts, recognition), communication & transparency (C0), and the
> governance dilemmas pre-resolved at the constitutional level. It feeds the value
> substrate (V1–V4) and the `A1/A3/E4` meta-models. Implementation has **not** started.

---

## 0. The one idea everything hangs on

**Valuation is a process with epistemic states, not a number stamped at transaction
time.** What looks valuable now may be re-scored as anti-value later. Therefore every
governing mechanism below is built to be *revisable, attested, and transparent*, never
final-on-first-judgment.

A Value Flow's valuation lifecycle:

```
provisional  →  attested  →  settled  →  revalued
(producer      (independent  (window     (new evidence
 claims Æ)      beneficiary   closes,     reopens &
               confirms)      booked)     adjusts ledger
                                          + TrackRecord)
```

The state **steers on settled value and trends; it reacts cautiously to provisional
value** (acting hard on un-attested value causes policy whiplash).

---

## A0 — Principles (constitutional invariants)

These compile into `A1 State/Constitution` and `E4 ControlPolicy` as checkable rules.

1. **Imbalance is the only governing signal.** The state corrects measured imbalance in
   the Æ-vector; it maximizes no single axis (incl. `$`). No axis may be optimized below
   another's constitutional floor.
2. **Value is declared, attested, and revisable.** Append-only ledger; **revaluation is
   a first-class event**, not a deletion.
3. **Anti-value is symmetric to value and usually delayed & diffuse.** Booked at edge
   level *and* as systemic charges over patterns, attributed back via a *responsibility
   share*.
4. **Weights are democratic; accounting rules are not.** Citizens vote the *weights* of
   value dimensions; they do **not** vote the *rules of measurement*. Constitution sets
   floors/ceilings; citizens steer inside the corridor.
5. **Transparency by construction.** Every agent's logic, every vote, every revaluation
   is publicly reproducible. A decision that can't be reconstructed from public state is
   **void**.
6. **Subsidiarity.** Balance at the lowest competent level; only cross-region imbalance
   escalates.
7. **Power and reputation decay; concentration self-charges.** Autonomy = f(TrackRecord),
   revocable. Concentration of value *or* decision-power auto-triggers an anti-value
   charge — **and this applies to the state's own organs (Sub-Agents, parties, the
   operator), not only to citizens/BigTech.**
8. **The state generates demand, it does not command supply.** Sub-Agents pull toward
   balance via incentives/missions; citizens remain autonomous transformers.
9. **Meaning is a protected dimension.** The `meaning` axis has a floor that cannot be
   traded away even when economically optimal.

### New principles from the 2026-06-28 dialogue

10. **Cohort floors are non-votable (minority protection).** Imbalance is measured as a
    *distribution across cohorts*, never only in aggregate. Constitutional floors apply
    **per cohort**. The majority cannot vote a minority below floor: the system
    structurally **cannot register "balanced" while any cohort is below floor**. (See §B0.1.)
11. **Net effect across all cohorts is always measured and published (symmetry of harm).**
    A policy that protects a minority while pushing the majority below floor is *as
    visible and as charged* as the reverse. No harm hides behind framing. (See §B0.1.)
12. **Influence is earned, transparent, and non-purchasable (anti-propaganda).** Reach is
    equalized by construction; every source carries a verifiable, falsifiable track
    record; the state **annotates, it does not censor**. (See §B0.3.)
13. **Generosity outranks accumulation.** Producing value and *not consuming it* (donating
    it) books additional value — the gradient of the system points toward solidarity, not
    hoarding. Recognition is **peer-issued, not state-issued**. (See §B0.4.)
14. **Non-retroactivity / contemporaneous judgment.** Acts are judged by the norm-set
    (weights, corridors, pricing function) in force *when they were committed* — the
    value-flow analogue of no-ex-post-facto law. **Evidence updates retroactively; norms do
    not.** Revaluation re-prices with new evidence but contemporaneous norms.
    (See `Courts-and-Adjudication.md`.)
15. **Interpretive authority is rebuttable.** Value/anti-value are interpretable; a state
    agent's assessment is authoritative-by-default but **contestable in court**. Trust
    derives from transparency + calibration, not infallibility. No final unaccountable
    authority. (See `Courts-and-Adjudication.md`.)

---

## B0 — Organizational mechanics

Three layers: **Demos** (citizens) · **Executive** (Sub-Agents, one per Æ axis) ·
**Constitution + Council** (floors/ceilings, ratification, adjudication).

Four citizen primitives, each a public signed event on the Semantic Timeline:

| Primitive | Event | Maps to |
|---|---|---|
| Request a good | `NeedAnnounced` | B5 |
| Make a contribution | `ContributionMade` (→ Value Flow, claimed Æ) | C3 + V3 |
| Report value received | `ValueAttested` (realized Æ) | V3 |
| Vote on weights | `VoteCast` (priority budget over axes) | E4 + governance object |

Anti-gaming spine: producer **claims** Æ, independent beneficiary **attests** realized Æ;
the **claimed-vs-attested gap** is value leakage / hidden anti-value, and over-claiming
costs TrackRecord. Self-attestation is disallowed (BR2 analogue).

### B0.1 — Minority protection (the tyranny-of-the-majority problem)

**Honest framing: humanity has *tools* for this, not a clean solution.** The real-world
toolkit — entrenched rights removed from majority vote, supermajorities, federalism,
counter-majoritarian courts, proportional representation, consociational power-sharing
(Lijphart: mutual veto + segmental autonomy + proportionality) — each works partially and
each has failure modes (federalism doesn't help *dispersed* minorities; consociationalism
ossifies divisions; judicial review is itself contested).

**MOS has a structural advantage real democracies lack.** In a vote-counting democracy the
unit of decision is *headcount*, so minorities are structurally outnumbered. In MOS the
steering signal is **imbalance in the Æ-vector, measured per cohort** — which is
*independent of headcount*. A 2%-cohort below its floor generates a high-priority
imbalance the Sub-Agents must act on, **even if the majority voted to deprioritize that
dimension**, because floors are not votable (Principle 10).

Concrete mechanisms:
- **Distributional imbalance.** Imbalance = aggregate gap **+** cohort variance + any
  below-floor cohort. High variance / below-floor = systemic anti-value (ties Principle 7).
  The system cannot read "balanced" with a cohort under floor.
- **Equity / Ombudsman Sub-Agent.** A structurally independent guardian whose owned
  dimension *is distributional fairness itself* — senses cohort variance and below-floor
  cohorts, generates corrective demand. The counter-majoritarian organ.
- **Segmental autonomy.** Minorities hold authority over matters internal to them.
- **Supermajority + cohort veto** on changes to floors affecting that cohort.
- **Right to exit** (federation): a cohort can migrate/fork — a pressure valve and a check.

**Symmetry (Principle 11) — the hard, honest part.** Minority protection must not become a
lever by which a minority imposes *net* anti-value on the majority unchallenged. The model
makes the trade-off **explicit and measured rather than rhetorical**: any policy's net Æ
effect across **all** affected cohorts is computed and published; experts surface evidence
**both ways**; constitutional floors protect *everyone's* minimum simultaneously. The
contested-curriculum class of example is handled purely as **competing-harms measurement**
— the state takes no rhetorical side, it measures net effect per cohort and publishes the
evidence; floors for every cohort hold at once. This is a strength of value-flow
governance: the fight becomes an accounting question with public evidence, not a shouting
match.

### B0.2 — Parties (liquid / delegative democracy)

Most citizens don't want to vote on every weight and every strategic initiative forever.
**Parties** absorb that function. This is **liquid democracy**, with these properties:

- **Delegation is a first-class, revocable, scoped object.** A citizen delegates their
  weight-vote and/or value-assessment to a party.
- **Topic-scoped.** I can delegate my *ecological* weight to a green party while keeping my
  *economic* vote myself. (The key advantage over plain representative democracy.)
- **Instant revocability.** Withdraw anytime — no electoral term. Resume self-voting or
  switch parties freely.
- **Parties are value transformers, evaluated by their members.** A party *claims* to
  represent a priority set P; members *attest* whether its actual votes matched — a
  **representation-fidelity score** (direct reuse of the claimed-vs-attested gap).
- **Equal, structural channel to inform** (no money-amplified reach — Principle 12).
- **Concentration cap on delegated weight** (Principle 7): past a threshold, marginal
  delegated weight is **quadratically discounted**, keeping the polity poly-centric. A
  party cannot become a de-facto majority dictator by accumulation.
- **Bounded transitivity:** a party may sub-delegate to an expert, but transitivity depth
  is capped to prevent mega-concentration.

### B0.3 — Experts & information integrity (anti-propaganda)

Propaganda works in reality because **reach is buyable and source track-record is opaque.**
MOS removes both levers.

- **Expert = a Persona with a domain-scoped, verifiable Expertise Score**, *earned* from a
  track record of **calibrated, later-verified claims** — did their past assessments
  survive the observation window / revaluation? (Reuses the provisional→settled lifecycle:
  experts are scored by how well their provisional judgments held up.) A pseudo-expert
  whose predictions failed loses score, **fully traceable on the verifiable log** — any
  false expert can be brought to light.
- **Calibration scoring** (Brier/Tetlock-style): experts *stake confidence*; scored on
  calibration, not just direction. Gameable-resistant.
- **Undistorted, full delivery.** Expert opinions reach citizens in full, with provenance;
  no algorithmic amplification or suppression. Every item a citizen sees carries
  provenance + the source's verifiable reputation; **reach is not purchasable.**
- **Experts evaluate parties**, symmetrically: if a party advances a minority interest at
  net cost to the majority (or vice-versa), that is delivered to everyone **with evidence**
  (Principle 11).
- **Conflict-of-interest is on-ledger.** An expert's value-flows (who funds/connects to
  them) are public, so capture is visible.

**The landmine, stated plainly.** "Full, undistorted delivery of expert opinion" +
"managed influence" risks recreating a censor / technocracy (who decides expert vs
misinformation?). MOS's answer is **transparency, not censorship**: the system does not
suppress speech — it **annotates** every message with verifiable reputation + provenance
and **equalizes reach**. The state is never the arbiter of truth; it is the guarantor that
track records are honest and reach is fair.

### B0.4 — Contribution, generosity & peer recognition

- **Contribution → access asymmetry.** High TrackRecord lets a citizen *request* more value
  / scarce opportunity (B4). Requesting is a claim, not a taking.
- **Altruism multiplier (Principle 13).** Value produced, *not consumed*, and donated to
  others books **additional** Æ on `meaning` + `social_stability` — a *generosity flow*.
  Hoarding = concentration = anti-value; donating = value. The system's gradient points at
  generosity.
- **Peer recognition, not state honors.** Medals/achievements are **citizen-issued
  attestations**, not state awards. A recognition flow is *costly to the giver* (so it
  isn't spammed) and books meaning-value to the receiver; a recognition from a high-
  TrackRecord peer weighs more (quadratic to resist celebrity-gaming). The state only makes
  the recognition ledger visible. This matches the wish: **citizens, not the state, honor
  their best.**

---

## C0 — Communication & transparency

- **Agent↔agent:** A2A + MCP over the AIL (orkestro.net). Citizens (Persona) ↔ Sub-Agents
  (Position).
- **Civic event bus:** the public append-only Semantic Timeline (E2); all civic events
  signed (JWS/EdDSA, already in stack).
- **Public governance repo:** constitution, accounting rules, Sub-Agent prompts/policies in
  open git (`orkestron-ai`). Every Sub-Agent decision cites the **commit-hash** of the
  logic that produced it → reproducibility.
- **Open voting = reproducible tally.** After each round: pseudonymous votes + aggregation-
  function version (commit-hash) + resulting weight delta are published; a citizen can
  *replay* the count and see how their vote moved the weights.
- **Verifiable log, not a blockchain (P0–P1).** Hash-chain + Merkle the event journal
  (Certificate-Transparency style); publish periodic signed Merkle roots. Gives append-only
  tamper-evidence + public audit **without consensus/gas/throughput limits**. Real on-chain
  is reserved as an optional settlement adapter only for *cross-operator* federation (P2+).
  - *Note (per owner 2026-06-28): in a synthetic simulation, trust requirements are lower
    than reality — the verifiable-log-over-full-blockchain choice is marked as a deliberate
    technical simplification for the model.*
  - **Æ is a non-transferable accounting unit, not a tradeable coin.** The article is
    anti-concentration; naive token economies concentrate. No speculative token in the
    value substrate.

---

## Resolved vs still-open

**Resolved in this dialogue:**
- Q1 Axes — 9 axes accepted, to be **extended** (see Proposed axis change below).
- Q3 Tiers — Tier-A share is a **simulation dial (10%–90%)**: wake more of society when
  their interests are harmed, quiet them when society is comfortable for them.
- Q4 Region/federation — **single region for P0, but `region` + `cohort` are first-class
  fields from day one**; minority-vs-majority must still be simulated even in one region.
- Q6 Blockchain — **verifiable log now**, on-chain optional for federation; marked as a
  deliberate simplification.
- Q7 Voting — **liquid democracy: individual voting + revocable, topic-scoped party
  delegation**, with concentration caps.
- Q8 Git — **yes** (this repo).

**Still open:**
- Q2 Anti-value quantification — to be worked as a dedicated piece (edge vs systemic +
  responsibility share + detection lag).
- Q5 ELMM tie-in — owner will send context later; **not detailed/mature** (a light
  ChatGPT exploration). Provisional: model MOS as its own Dimension; don't block P0.

**Proposed axis change (for ratification).** Keep 9 axes; add **`epistemic` (information
integrity / health of the shared knowledge commons)** as a 10th axis, because
anti-propaganda is now central. Treat **distributional equity** and **generosity** *not* as
axes but as **cross-cutting constructs** — equity is a *floor-protected constraint +
guardian agent* (you must not be able to *trade it away* via weights), and generosity is a
*flow type*. Design discipline: **axes are the things you trade off via weights; things you
must never trade off are constraints/guardians, not axes.**
