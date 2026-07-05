# Axiacracy — Full Specification

| | |
|---|---|
| **Status** | **DRAFT — the complete, self-contained description of the doctrine** |
| **Purpose** | The definitive exposition. Read **this** (not the terse compendium) for an unambiguous understanding. Every mechanism is given a **definition → rationale → how it works → a worked example (from the Meta-Orchestrator State simulation, "MOS") → what it is NOT**. |
| **Reflects** | the v2 "sensing vs. coercion" synthesis. |
| **Updated** | 2026-06-28 |

> **How to read this.** Axiacracy has been repeatedly *misread* by reviewers who saw a short
> summary and filled the gaps with the nearest cliché (central planning, social credit, a
> single imposed value score). This document exists to remove that ambiguity. If a passage
> seems to say something authoritarian or naïve, check the **"What this is NOT"** note attached
> to it — the misreading is almost certainly pre-empted there.

---

## 0. Seven misreadings, pre-empted up front

Before the details, the seven errors reviewers most often make — and the correct reading:

1. **"The state computes one number for 'civilizational value' and optimizes it."**
   ✗ No. The state **senses** value across many dimensions (a dashboard), and the Æ-vector is
   **the state's own weighted viewpoint — one frame among many, openly political and
   revisable** — not a universal truth and not a scalar it maximizes. Crucially, **sensing is
   separated from coercion** (Part III): the state may *see* broadly but may *compel* only
   narrowly.

2. **"It's central planning — the state allocates resources."**
   ✗ No. **Markets keep doing allocation.** The state only **prices the residual that markets
   miss** (externalities) and **guarantees material floors**. Hayek's knowledge problem is
   respected: the state *supplements* prices, it does not *replace* them.

3. **"Value is self-reported, so it's trivially gamed / it's social credit."**
   ✗ Self-report (attestation) is only **one cross-checked, staked input** among many
   (objective side-effects, revealed behaviour, third-party sensors, prediction markets), with
   collusion-detection and **retrospective revaluation** (an anti-Goodhart device). Measurement
   is treated as an **adversarial-security problem**, not a trusted oracle.

4. **"The state measures your meaning / inner life — mind-monitoring."**
   ✗ Meaning is **sensed in aggregate but never coerced on**, and floors are defined as the
   **availability of material means to function**, *not* an audit of whether you *feel*
   fulfilled. An ascetic who chooses a "low-functioning" life is free.

5. **"Rent = captured − created is an uncomputable counterfactual."**
   ✗ That metaphysical formula is **not** the operational test. Rent is priced from
   **observable signatures** (returns durably above the competitive/risk-adjusted norm,
   monopoly pricing power, location value by comparables, clear-title resources, network-effect
   capture) — narrow, auditable categories.

6. **"Retrospective clawback means nothing is ever final — economic chaos."**
   ✗ Clawback is **bounded**: a statute of limitations for honest (non-concealed) harm,
   **fixed-rate insurance-style premiums** instead of continuous recomputation, and
   **systemic-risk throttles**. Perpetual liability applies **only to concealment/fraud**.

7. **"Æ is a token / cryptocurrency."**
   ✗ Æ is a **non-transferable accounting record** (like a credit history, not a coin). It
   cannot be bought, sold, or inherited. This is deliberate — it prevents wealth from directly
   buying civic power.

---

# Part I — Foundations

## 1. The problem Axiacracy answers
For two centuries, states assumed **human labour is the basis of economic value**, and built
everything (tax, welfare, labour law, national identity) on it. AI breaks that assumption:
economic output can keep rising while human participation in production falls. The industrial
feedback loop — **labour → income → consumption → tax → redistribution** — begins to collapse:
labour income falls, consumption weakens, tax bases erode, and value concentrates around the
owners of AI infrastructure. Yet society still needs food, housing, health, energy, education,
stability, science, and demographic continuity.

Two dangers dominate this transition:
- **Concentration** — whoever owns computation, models, data, logistics and robotics can
  capture a runaway share of value.
- **Loss of meaning** — if humans become economically optional, the deepest risk is not
  unemployment but the collapse of purpose, status, and belonging that work used to provide.

GDP cannot see either danger: a platform can add trillions in market cap while degrading
attention, destroying professions, and weakening communities. **Financial success ≠
civilizational success.** Governance therefore needs to see and steer by **multidimensional
value**, not money alone.

## 2. The core reframe: a graph of value transformers
Axiacracy stops seeing society as *taxpayers, employees, corporations, consumers*. It sees a
**graph of value transformers** — citizens, families, businesses, AI systems, institutions,
cities, infrastructure, agents — each of which continuously **consumes, transforms, creates
value, or generates anti-value**. Governance becomes the **coordination and balancing of the
value flows** between these transformers, measured across many dimensions, not the collection
and redistribution of money.

*MOS example:* a teacher (transformer) consumes value (food, tools, prior knowledge), transforms
it (teaching), and creates **educational** and **cognitive** value in a student (another
transformer). A social-media platform creates **economic** value and, simultaneously, may
generate **cognitive anti-value** (attention erosion) — the same flow carries both, on different
axes.

## 3. What Axiacracy is — and is not
- **Is:** a doctrine (called **Axianomy** as a discipline) for governing a polity by *seeing*
  multidimensional value and *balancing* its flows, with money demoted from sovereign to
  instrument, and with coercion strictly disciplined by how well things can be measured.
- **Is not:** central planning (markets keep allocating); a single imposed value score (the
  Æ-vector is the state's *own* weighted lens, and it never coerces on unmeasurable
  dimensions); social credit (transparency is a *constraint on power*, sensing is
  privacy-bounded, and there is no secret behavioural score used to punish); money abolition ($
  survives as one axis and a settlement rail); or a finished blueprint (it is a research
  programme whose simulation exists precisely to find where it breaks).

---

# Part II — The Value Substrate (V1–V5)

These five foundational meta-models are the vocabulary everything else is built from.

## 4. V1 — Value Transformer
**Definition.** The universal node type: *any* entity modelled as something that consumes,
transforms, and creates value, or generates anti-value. Every object in the system (citizen,
ministry, company, family, city, agent) **is** a value transformer.
**Why.** It gives one uniform way to reason about wildly different actors: all of them are
nodes in the value graph.
**How.** A transformer has inflows (value it receives), outflows (value it produces), a
conversion behaviour, and a reputation/standing record.
**MOS example:** a citizen-agent on the Agent Hub is a Persona (identity + competencies) bound
to a transformer record; its "job" is a role (Position) that specifies what value it is expected
to transform.
**Not:** not a "worker" or "taxpayer" — those are narrow economic roles; a transformer includes
non-market value (a parent creating demographic and meaning value creates real value even with
no wage).

## 5. V2 — Multidimensional Value (the Æ-vector)
**Definition.** Value is a **vector across ten dimensions (axes)**, not a scalar:
`economic · educational · scientific · demographic · cognitive · infrastructural ·
social_stability · ecological · meaning · epistemic`. Alongside it runs an **anti-value** vector
(V4). The unit is a value-point on each axis.
**Why.** GDP collapses all value to one axis (money) and is therefore blind to the very things
that matter most in the AI transition (meaning, cognition, demographics, epistemic health). A
vector keeps them visible and separately accountable.
**How — and the crucial clarification about "commensurability":** to *compare a current state
to a target* the system computes a **weighted distance** in this vector space, using a weight
vector `w(t)`. **`w(t)` is not a metaphysical exchange rate claiming "1 unit of education = 1
unit of money."** It is an **openly-declared political priority**, set by democratic vote,
revisable each period, and it is **the state frame's own** weighting — not a universal truth
binding on anyone else. Measuring many things on named scales does **not** assert they are
morally reducible to one thing, any more than physics measuring both temperature and entropy
claims they are the same.
**The ten axes, each briefly:**
- **economic** — production, trade, services (money is *this* axis, and only this axis).
- **educational** — teaching, skill transfer, mentorship.
- **scientific** — research, discovery, verified knowledge.
- **demographic** — households, care, births, age-structure health.
- **cognitive** — attention, deep work, problem-solving capacity (its anti-value: dependency,
  attention erosion).
- **infrastructural** — energy, logistics, compute, housing, resilience.
- **social_stability** — cohesion, trust, low conflict.
- **ecological** — emissions, resource balance, restoration.
- **meaning** — purpose, belonging, culture, identity (the article's central human axis).
- **epistemic** — integrity of the shared knowledge commons (its anti-value: propaganda,
  misinformation).
**Corridors.** Each axis carries, per cohort and region, a **floor** (a guaranteed minimum), a
**target band** (where the state tries to keep it), and a **ceiling** (a soft cap above which
extra value is discounted — the anti-concentration device on the economic axis).
**MOS example:** the state's dashboard shows the cognitive axis for a youth cohort trending
down while economic is up — a signal invisible to GDP but central here.
**Not:** *equity* and *generosity* are deliberately **not axes** — equity is a floor-protected
constraint (you must not be able to *trade it away* by re-weighting), and generosity is a *type
of flow*. Design rule: **axes are what you trade off via weights; what must never be traded off
is a constraint, not an axis.**

## 6. V3 — Value Flow (and its lifecycle)
**Definition.** The edges of the graph: a transfer/transformation of value from a source
transformer to a sink, carrying an Æ-delta (per axis), a cost, a time, and provenance.
**The lifecycle (this is load-bearing — value is a *process*, not a stamp):**
- **Planned value** — what the *producer* claims the flow is worth (the sender's interpretation).
- **Realized value** — what the *recipient* actually experiences (the receiver's interpretation),
  confirmed by an independent beneficiary. Value is *realized at consumption*, not at claim.
- **Retrospective value** — a later re-scoring when new evidence arrives (e.g., a harm surfaces).
- **Flow resistance** — the gap between Planned and Realized; it accumulates and is itself a
  signal (a producer who chronically over-claims builds resistance and loses standing).
- **Leakage** — value that persistently exits a subsystem more than enters (a sign of parasitism).
**MOS worked example — the yogurt:**
1. You take a yogurt; the checkout records the item and its standard value-cost. This books a
   **provisional (Planned)** flow: business → you, +nutritional value, −economic (you draw
   entitlement). *Zero ceremony.*
2. No complaint within the window → the flow **auto-settles** as Realized. Done. ("Silence =
   attestation" — **but only for low-stakes routine goods.**)
3. The yogurt was spoiled and made you ill → you file a **reclamation** (`ValueDisputed`). The
   realized value is negative; the business is charged **health/social anti-value** proportional
   to harm and refunds you; its quality record drops. This is the **Retrospective** re-scoring.
**Not:** value is never a number fixed at the moment of sale; a sale that looked positive can be
re-scored negative later — legitimately, because we *learned* what actually happened.

## 7. V4 — Anti-Value
**Definition.** Systemic and local harms as **first-class objects — an independent category, not
merely "zero" or "negative" value.** A single flow can carry **both** real value and real
anti-value at once (a productive-but-harmful platform), booked on separate axes and **not netted
away** in the ledger.
**Classified three ways:**
- **Scope** — *edge* (attributable to one flow, e.g., the spoiled yogurt) vs *systemic* (emerges
  from a pattern over many flows, e.g., content dependency — no single video harms you).
- **Detection lag** — *immediate* (pollution at the smokestack) · *short* (a service failure) ·
  *long* (dependency, cognitive erosion) · *generational* (demographic decline). Lag decides the
  enforcement instrument (immediate → charge now; long → retrospective).
- **Intent / kind** — *rights-violation* (murder — **not priced**, criminal law) · *malicious*
  (fraud) · *self-directed/distress* (addiction — **care, not punishment**) · *negligent*
  (externalities without intent — priced).
- **Responsibility share** — for systemic harm caused by many actors, blame is apportioned
  (proportional to each actor's contribution; heavier if the contribution was concealed).
**MOS examples (three profiles across the whole lifecycle):**
- **Spoiled yogurt** — edge, short lag, 100% one business.
- **Content dependency** — systemic, long lag; each session looks fine (Planned/Realized neutral),
  but the *pattern* over months erodes cognition and meaning (Retrospective negative), apportioned
  across attention-capturing platforms.
- **BigTech concentration** — systemic, continuous + long lag; genuinely productive
  (Planned/Realized positive to customers) yet accumulates value/power (Retrospective: economic,
  social, dependency anti-value from the *accumulation*, not any single deal).
**Not:** anti-value is not the mirror-image of value on one scale; an actor can be **high value
AND high anti-value simultaneously**, and the ledger must show both, not blur them into a
mediocre middle.

## 8. V5 — Value System / Frame (and why there is no "apex")
**Definition.** Following Value Management Theory (VMT), a **value system is a frame of reference
`{A, F, G, R, T}`** — a set of actors, flows, improvement/degradation criteria, interpretation
rules, and a time horizon. **Value exists only inside a value system;** the same act has
different value in different systems.
**Consequences (the pluralism claim, made precise):**
- **Every** citizen, family, business — and the **state itself** — is a value system with its
  *own* weights and criteria.
- The polity is a **federation of value systems**, not a hierarchy with one at the top. There is
  **no "value in general"**; you cannot sum all frames into one master number (that would be a
  category error). Systems interact **only at their boundaries, via external flows.**
- **The state is one frame with a bounded mandate — not the owner of all value.** Its Æ-vector is
  *its* lens for *its* interventions; it does **not** reach inside other frames to measure or
  overwrite their internal value.
- **Participation condition θ** — each actor stays in the system only while its participation
  condition holds. If the state's actions make an actor's θ fail (it becomes unsustainable for
  them to remain), that is a **first-class alarm on the state**, not a fault of the actor. A
  polity is sustainable only while all actors' θ hold.
**MOS example — a religious/traditional community:** the state *senses* their activity in its
axes and may score it low on, say, "economic." That does **not** trigger punishment. The state
**cannot coerce** them on subjective/internal-to-their-frame matters; it acts only at genuine
cross-boundary harms and to guarantee material floors (which *help* the community exist, not
erase it). Their θ is protected; pluralism is preserved **operationally**, not just rhetorically.
**MOS example — a family:** the family is its own value system (its criterion G might be
"everyone gets along"). By the boundary rule, the state sees only the family's *external* flows
(demographic output, wellbeing signals crossing the boundary), never the dinner-table interior.
If the state wants higher birth rates, it must make family life sustainable **from the family's
own point of view** (lower its internal stress, meet material floors) — never impose its frame
inside the home.
**Not:** "federation of frames" is not window-dressing over a single central metric — the state
is *operationally* barred (Part III) from coercing on internal-frame value, which is what makes
the non-apex claim real rather than rhetorical.

---

# Part III — The Governing Stance (the heart of the doctrine)

This is where the three-panel critique was answered, and where most misreadings live. Read it
slowly.

## 9. Sensing vs. Coercion — the central distinction
The doctrine draws a hard line between two things that critics (and earlier drafts) conflated:

- **Sensing** = *seeing* multidimensional value — building the civilizational dashboard. This is
  **observation**. It is **not** an exercise of power over anyone, and it is the founding
  revolution: *stop being blind to non-GDP value.* Sensing is **rich across dimensions.**
- **Coercion** = *compelling* — charging anti-value, enforcing a floor, redirecting resources,
  restricting access or liberty. This is where legitimacy, gaming (Goodhart), and collusion
  bite. Coercion is **strictly bounded.**

**The founding idea (seeing value beyond GDP) lives entirely in the sensing layer and survives
whole. Only coercion is disciplined.** Reviewers who called Axiacracy a "measurement tyranny"
assumed that *measuring* something licenses *compelling* on it. It does not.

**Sensing is nonetheless bounded too** (measurement has social costs — even un-acted-upon
surveillance chills behaviour): by default sensing is **cohort-aggregate**, privacy-budgeted,
with individual-level detail only by the individual's consent, and with forbidden inferences
(you may not derive protected attributes from value-frame data).

## 10. Graduated coercion = f(measurement-confidence × inter-frame scope)
The state's **power to compel scales with (a) how confidently the thing can be measured and (b)
how far the harm crosses between frames.** Concretely:

| Situation | Coercion allowed? | Instrument |
|---|---|---|
| High-confidence, objective, **inter-frame** harm (e.g., measured pollution crossing to others) | **Yes** | charge / restriction (escalation ladder) |
| A **material floor** is breached for a cohort | **Yes** | compel provision to restore the floor |
| Low-confidence or **subjective** or **intra-frame** matter (e.g., a lifestyle scored low on "meaning") | **No** | **soft power only**: publish the signal, offer incentives, illuminate — never compel |

This is a **constitutional dial tying power to epistemics.** It is the direct answer to
"measurement tyranny" and "apex metric": **the state may *see* meaning, but may never *compel*
on it**, because meaning cannot be objectively measured and is internal to frames.

**MOS examples:**
- The state measures a factory's emissions (objective, inter-frame) → it may **charge** the
  ecological anti-value.
- The state notices a subculture scores low on its "meaning" axis (subjective, intra-frame) →
  it may **only** publish aggregate signals and offer opt-in support; it may **not** penalize,
  nudge-out, or restrict the subculture.
- A cohort falls below the **material** health floor → the state may **compel** provision of the
  missing material means (clinics, nutrition), because the floor is objective and material.

## 11. Measurement as adversarial security (not an oracle)
Because the whole system's inputs are measurements, and adversaries will attack them,
measurement is designed like a **security system, continuously red-teamed** — never assumed
correct.
- **Multi-source, cross-checked.** No single self-report is trusted. Signals combine: **objective
  side-effects**, **revealed behaviour** (what actors actually, costly-ly do), **independent
  third-party sensors**, and **prediction markets on outcomes** (a belief-aggregation /
  futarchy-style layer).
- **Attestation is staked.** Beneficiary attestation is *one* input; over-claiming or false
  attestation costs standing (skin in the game), and closed loops of mutual attestation are
  flagged by **collusion-graph anomaly detection.**
- **Retrospective revaluation is an anti-Goodhart device.** You cannot *durably* game a metric
  that is **re-judged later with hindsight** — the gain from gaming is clawed back when the true
  effect surfaces.
- **Confidence is explicit and gates action.** Every estimate carries an uncertainty; the state
  acts hard only on high-confidence estimates (per Part 10), and treats low-confidence ones as
  provisional (illuminate, don't compel).
**MOS example — a collusion ring attack:** 40 agents mutually attest high value for trivial
outputs. Detection: their attestation graph is an almost-closed loop with little external
validation → flagged; their revealed behaviour (no third party actually uses the outputs) →
contradicts the claims; a prediction market on "will this output be used?" prices it near zero;
and if it slips through, retrospective revaluation later strips the standing they gained. The
ring's cost/benefit is engineered to be negative. **The simulation's central job is to test
exactly this — where such defences hold and where they fail.**
**Not:** the doctrine does **not** claim measurement is solved or that Æ is objectively knowable.
It claims measurement is an *ongoing adversarial engineering problem*, and it builds the sim to
map the frontier of what survives gaming.

## 12. The escalation ladders (how coercion actually lands)
Where coercion *is* permitted (Part 10), it is applied as a **graduated ladder across
lower-bound thresholds**, not a single automated punishment. Crossing successively worse
thresholds triggers, in rising order:

**annotation → charge / fine → access & standing restriction → loss of liberty (criminal).**

Each threshold, and its penalty, is **defined per polity (implementation)**; the **principle**
(graduation, proportionality, only on defensible inter-frame/floor measurement) is universal
(Charter). Different *kinds* of harm ride *different* ladders — a criminal sanction, a civil
liability, an administrative restriction, and a reputational annotation are distinct, **not one
merged automatic debt.**
**MOS example:** a business with rising, measured spoilage first gets its record **annotated**;
persistent harm → **charges** + escrow forfeit; gross, ongoing harm → **restriction** of access
to scarce inputs; fraud/concealment (a rights-adjacent crime) → the **criminal** ladder via the
courts.

## 13. How Part III answers the three classic attacks
- **Hayek (you can't centrally compute the economy):** markets keep allocating; the state only
  prices the *residual* markets miss and guarantees floors — it *supplements* prices, never
  replaces them.
- **Goodhart (any optimized metric is gamed):** multi-source + staked + anomaly-detected +
  retrospectively revalued measurement, and — decisively — **coercion is withheld where
  measurement is weak**, so there is little to game where gaming is easy.
- **Pluralism/apex contradiction:** the state is *operationally barred* from coercing on
  internal-frame value; it acts only at boundaries and floors; so its frame is not the apex owner
  of value, in practice, not just in words.

---

# Part IV — The Governing Loop (operational)

## 14. One tick, step by step
The state runs a continuous cybernetic loop. One tick, with an MOS scenario threaded through:

1. **Sense (richly).** Update the Æ dashboard from multi-source measurement. *MOS:* the
   cognitive axis for a youth cohort is drifting below its target band; economic is fine.
2. **Diagnose imbalance.** Compute the imbalance signal:
   `imbalance = Σ over axes [ w_a · distance(current_Æ, target_band) ] + below_floor_penalty +
   variance_penalty(across cohorts)`. Two of these terms are **not** scaled by the voted weights:
   the **below-floor penalty** (a cohort under floor is a large signal regardless of how the
   majority weighted that axis) and the **cross-cohort variance penalty** (inequity is itself a
   flagged harm). *MOS:* the youth-cohort cognitive drift is within-band but trending; no floor
   breach yet → a *soft* signal, not a coercive trigger.
3. **Attribute cause.** Trace the flows driving the drift. *MOS:* attention-capture by a few
   content platforms correlates with the cognitive decline (systemic anti-value, long lag).
4. **Generate strategic demand.** The relevant Sub-Agent (here, a Cognitive-Health ministry)
   proposes responses. Because the signal is subjective-ish and intra-frame-heavy, the response
   is **soft**: publish the trend, fund cognitive-development programs, offer incentives for
   platforms to change engagement design — **not** a ban.
5. **Respond (graduated).** Apply Part 10/12: soft power here; coercion only if/when a *material*
   or *inter-frame* threshold is crossed (e.g., a platform's measured, concealed harm passes a
   charge threshold).
6. **Re-sense.** Next tick, observe whether the drift corrected. Hysteresis prevents overreaction
   (the weights and targets can't swing more than a bounded amount per period).

**Not:** the loop does **not** mechanically punish whatever scores low. Most of its output is
*information and incentives*; coercion is the rare, high-confidence tail.

---

# Part V — Governance Mechanics (how citizens actually govern)

## 15. The civic loop — four public, signed events
Citizens govern through four event types, all published to a public, tamper-evident log:
- **`NeedAnnounced`** — a citizen declares a need (bottom-up demand).
- **`ContributionMade`** — a citizen does something; it books a value flow with a **claimed**
  (Planned) Æ-delta.
- **`ValueAttested`** — an *independent beneficiary* confirms the **realized** Æ; the gap between
  claimed and attested is flow resistance; the attestation is **staked**.
- **`VoteCast`** — a citizen distributes a priority budget across the ten axes (this is how
  `w(t)` is set).
**MOS example:** a mentor logs `ContributionMade` (+educational to a student); the student logs
`ValueAttested` confirming what they actually learned; if the mentor over-claimed, resistance
accrues and standing drops.

## 16. Weights, corridors, and liquid democracy
- **Weights** `w(t)` are set by vote — an open political choice of what the polity currently
  prioritizes, revisable each period, change-rate-limited (hysteresis).
- **Corridors** (floor / band / ceiling) per axis, per cohort: the **existence** of floors is
  constitutionally entrenched; their **level** is democratically set; floors are **non-votable
  downward per cohort** (minority protection, §19).
- **Liquid democracy.** Most citizens don't want to vote on everything, so they may **delegate**
  their weight-vote to a **party** — revocably and **topic-scoped** (delegate your ecological
  vote to a green party while keeping your economic vote yourself). Vote cost is **quadratic**
  (intensity is expressible but expensive), individual weight is reputation-influenced but
  **capped**, and a party's accumulated delegated weight is **quadratically discounted past a
  threshold** so no party becomes a dictator by accumulation.
**Not:** parties are not permanent representatives with fixed terms — delegation is withdrawable
instantly, and parties are themselves scored on how faithfully their votes matched what their
delegators wanted (a representation-fidelity measure).

## 17. Experts and information integrity (anti-propaganda)
Propaganda works because **reach is buyable** and a **source's track record is opaque.** Axiacracy
removes both levers:
- An **expert** has a domain-scoped **calibration score** (Brier-style): they stake confidence on
  claims, and are scored on whether their past assessments held up. A pseudo-expert whose
  predictions failed loses score, publicly.
- **Reach is not purchasable**; every message a citizen sees carries the source's verifiable
  track record and provenance.
- The state **annotates, it never censors** — it attaches verifiable reputation to speech rather
  than suppressing it. Conflicts of interest are on the public ledger.
**Not:** this is not a "ministry of truth." The state does not decide what is true; it guarantees
that *track records are honest* and *reach is fair*, and lets citizens judge.

## 18. Recognition and generosity
- **Recognition** (honours, "medals") is **peer-issued, not state-issued.** A citizen can grant
  recognition to another; it is **costly to the giver** (so it isn't spammed), **weighted by the
  giver's own standing**, and **dampened by network-centrality + decay** so localized praise
  cannot snowball into macro power (closing the "patronage network" attack).
- **Generosity multiplier.** Value you produce, do not consume, and **donate** books *additional*
  value on the meaning/social axes. The system's gradient therefore points toward **giving, not
  hoarding.**

## 19. Minority protection (why the majority can't crush a minority)
In ordinary majority-vote democracy the unit of decision is *headcount*, so minorities are
structurally outvoted. In Axiacracy the governing signal is **imbalance measured per cohort**,
which is **independent of headcount**:
- Floors apply **per cohort** and are **not votable downward.** A 2%-cohort below its floor
  produces a **large imbalance signal** the state must address **even if the majority
  de-prioritized that axis** — because the below-floor penalty is *not* scaled by the voted
  weight (§14).
- An **Equity/Ombudsman guardian** watches cross-cohort variance as its own mandate.
- **Symmetry of harm:** a policy that protects a minority while pushing the majority below floor
  is *as visible and as charged* as the reverse; net effect across **all** cohorts is measured
  and published. The trade-off becomes an accounting question with public evidence, not a
  shouting match.
**Not:** minority protection is not a majority favour that can be voted away; it is a structural
property of the imbalance signal itself.

---

# Part VI — The Economy (value, money, markets, property)

## 20. Two layers: the sovereign Æ-ledger and the money rail
Axiacracy separates two things money normally fuses:
- **The sovereign layer — the Æ-ledger.** A **non-transferable** accounting of value and
  anti-value. It records what you have contributed and received across the axes. It is **like a
  credit history, not a coin**: it cannot be bought, sold, gifted, or inherited. This is what
  prevents wealth from directly buying civic power (anti-plutocracy).
- **The convenience layer — a settlement rail (money, `$`).** Fast, impersonal, low-ceremony —
  for routine exchange. Money is **one axis (economic) plus a settlement instrument**, not the
  sovereign measure.
**Why demote money without abolishing it?** Money is unbeaten at low-ceremony routine settlement
(buying a yogurt), so it stays as the *rail*. But it is blind to the other nine axes and to
externalities, so it is *not* the thing the state steers by.
**Not:** Æ is not a currency or token; you cannot get rich by accumulating Æ, and you cannot
transfer it to a friend.

## 21. Consumption and settlement (avoiding a bureaucratic quagmire)
Accounting every consumption act in full would drown the system in bureaucracy. So **ceremony is
proportional to stakes:**
- **T0 (ambient)** — routine, low-stakes (a yogurt): the checkout records what you took; it
  **auto-settles**; **silence = attestation.**
- **T1 (attested)** — a service, a course: a lightweight beneficiary attestation.
- **T2 (reviewed)** — high-stakes or disputed: full independent review, possibly a court.
The heavy machinery fires **only at T2.** Quality is policed by **exception** (reclamations) and
by **statistical audit**, not by inspecting every transaction. Crucially, **"silence =
attestation" applies only to T0 low-stakes goods** — for contested or high-stakes goods, positive
value requires *active* confirmation, with random audits and consumer protection that favours the
weaker party.
**Why the simulation escapes the quagmire that would sink a real bureaucracy:** in the sim,
*recording* a transaction is free (it's data); only *judgement* costs (agent attention), and
judgement is reserved for T2. In reality the same design shifts the cost from human paperwork to
targeted review.

## 22. Markets and the externality overlay (multidimensional Pigou)
- The **market clears allocation.** Citizens direct their earned entitlement to the businesses
  and providers they choose; **the citizen's choice is the reward.** The state does not decide
  which business deserves value. This preserves market discovery (Hayek).
- The **state prices the residual the market missed** — the externalities on the *other* axes.
  Every business↔citizen transaction produces **two bookings:** (1) the **market booking**
  (immediate, `$`, the citizen's choice) and (2) the **civilizational booking** (the state prices
  only the externality residual — pollution, dependency, concentration, or positive spillovers
  like education). This is **Pigou generalized from one axis to ten.**
- **Profit is decoupled from civilizational value.** A profitable-but-harmful actor has high `$`
  inflow and high anti-value → low or negative *net* civilizational value → it **loses standing
  and access even while profitable.** This is the article's BigTech-balancing, mechanized.
- **The vote-vs-spend gap** (what citizens *vote* as priority vs what they *spend* on) is a
  first-class diagnostic — the state does not force them to agree; a systematic gap is a signal
  to reshape the *incentive field*, never to ban the spending.
**Not:** the state is not a central planner choosing production; it is a *referee pricing
externalities* over a market it does not run.

## 23. Value↔money coupling — instant + retrospective, but bounded
How does anti-value actually bite money — without the slow real-world chain of
discontent→politicians→laws→antitrust→redistribution (during which the harm is already done)?
By putting anti-value and money **in the same ledger, cleared the same tick.** The instruments
(not discretionary fines) are:
- **Externality escrow** — a fraction of a business's inflow is withheld against its externality
  exposure; you cannot bank revenue whose externalities haven't settled.
- **Continuous anti-value debit** — measured anti-value is debited the same tick.
- **Concentration charge** — accumulation above the ceiling self-charges.
- **Standing/access loss** — a poor quality record gates access to scarce inputs.
- **Retrospective clawback** — for harms that surface late.
**Bounded, to keep the economy predictable (answering "retroactive chaos"):** a **statute of
limitations** for honest (non-concealed) harm; **fixed-rate insurance-style premiums** instead of
continuously recomputed liabilities; **systemic-risk throttles** (transition bands, insurance,
bankruptcy, no synchronized clawback that collapses a whole sector at once). **Perpetual
liability applies only to concealment/fraud** — because concealment violated the norms of its own
time (so it isn't retroactive punishment).
**MOS example — BigTech:** a platform pays escrow scaled to its externality exposure; its measured
attention-harm is debited continuously; its accumulation above the ceiling is charged; if it
*concealed* engagement-harm, a later clawback recovers the ill-gotten standing/assets and routes
them to the harmed cohorts (education, cognitive-health programs).

## 24. Property, rent, and the commons
**Principle: you own what you create (earned value); you do not own what nature or society
created (unearned rent).** This is neither capitalism (which lets rent be captured privately) nor
socialism (which collectivizes even earned value).
- **Earned → private.** Value you genuinely created is yours.
- **Unearned rent → commons.** Value you captured without creating — from **nature** (land,
  resources), **society** (network effects, location value, the knowledge commons), **position**
  (chokepoints), or **concentration** (monopoly) — is commons-owed.
- **Operationalized by observable signatures, NOT a counterfactual.** Rent is detected as:
  returns durably above the competitive/risk-adjusted norm; monopoly pricing power; location
  value assessed by comparables; resources/spectrum with clear title; network-effect capture.
  These are narrow, auditable categories — *not* an attempt to compute "what you would have
  created otherwise."
- **AI-compute/data/network-effects = the new "land".** Their value comes largely from humanity's
  collective data + public science + network effects, not solely from the owner → the unearned
  portion is commons-owed → funds a **citizen dividend + civilizational reinvestment** (exactly
  the article's "mandatory contributions to education, cognition, science").
- **Renting is not parasitism.** Renting out a produced asset (a car, tools, a **building's
  structure**) is **earned service income** — you provide use-value and bear depreciation/risk.
  Only the **land/location/scarcity/monopoly** component is unearned. **Inheritance:** goods are
  bequeathable, but land-rent stays commons-owed, the concentration ceiling caps dynasties, and
  Æ/standing cannot be inherited (you inherit goods, never civic power).
**Not:** this is not confiscation of profit; profit from *creation* is protected — only *rent*
(gains not traceable to creation, by observable signatures) is commons-owed.

## 25. Distributive justice — capability floors (availability, not audited feeling)
Axiacracy's stance is **capability sufficientarianism + a bounded, contribution-responsive band +
an anti-concentration ceiling + a generosity premium** — which is exactly the corridor
(floor/band/ceiling), now grounded in the Sen/Nussbaum **capability approach**:
- Floors guarantee a **threshold of central capabilities** — but defined as the **availability of
  the material/infrastructural means to function**, **not** an audit of whether you *achieved* or
  *feel* a functioning. (This is the precise fix to "mind-monitoring": the state ensures you
  *can* be healthy/educated/connected; it does not measure your inner state or push you to use
  the means.)
- Because people convert resources into capabilities differently (a disabled person needs more
  input for the same mobility), floors imply **equity of provision, not equality of inputs.**
- Above the floor, inequality is permitted (contribution-responsive) up to the ceiling.
**Not:** not egalitarian (inequality allowed above the floor), not pure meritocracy (a floor no
merit can revoke, a ceiling no merit can breach), not utilitarian (floors are lexically prior — a
below-floor cohort is never traded for aggregate gains).

## 26. Inter-frame value routing (a positive-sum superpower, privacy-bounded)
Knowing an actor's value frame (what *they* most value) lets the state:
- **pay them in their own currency** — give a scientist a hard problem + recognition (cheap to
  provide, highly motivating) instead of generic cash: positive-sum, value-creating;
- **monitor θ** — see when a valuable actor is about to disengage, and why;
- **match positive-sum flows markets miss** — compose a deal across frames (company wants talent,
  university wants funding, citizen wants purpose) that no money-market would assemble. The state
  is a **matchmaker/router, not an owner.**
This runs over **privacy-preserving frame disclosure:** a scoped access grant yields a **frame
summary** (derived from the actor's top realized flows), **never the raw ledger**; cohort-
aggregate by default; individual detail only by opt-in (for personalized benefit); with forbidden
inferences and consent revocation.
**Not:** this is not surveillance-for-manipulation. The state may **serve** your frame (offer what
you value, transparently, to accept or decline) but may **not rewrite** your preferences; the
line is transparency + consent + serving *your* goals.

---

# Part VII — Law and the State

## 27. The Charter and the hierarchy of norms
The **Charter** is the supreme document — a **meta-constitution (jus cogens)** that any polity
adopting Axiacracy instantiates and may **not contradict** (a conflicting law is **void**). It
has an **unamendable eternity core** (the value-balancing mandate, inviolable rights, floors,
anti-concentration, transparency/contestability) so the doctrine's own amendment process cannot
be used to abolish it — with a defined **constituent power** (a human body may replace the Charter
by deep supermajority, reconciling "no final authority" with the eternity clause).
```
Charter (universal principle) → State Constitution → Legal Codes (specific thresholds/penalties)
    → Regulations → individual rulings         (each conforms to the one above, or is void)
```
Its principle new in v2: **graduated coercion** — the state may compel only in proportion to
measurement confidence and inter-frame scope. **Charter = methodology (universal); the specific
coercion thresholds and ladders = implementation (per-polity).**

## 28. Rights, crime, and courts
- **Inviolable rights** (life, bodily integrity, liberty, consent, exit) are **not
  priceable/votable/tradeable** — their breach is a rights-violation, not a value transaction.
- **Crime is handled by KIND** (§7): rights-violations by criminal law (not priced); malicious
  harm by charges + bounded clawback; distress/addiction by **care, not punishment**; negligence
  by pricing. **Incapacitation** (imprisonment) is justified **not as retribution** but because a
  person whose continued participation makes *others'* participation conditions fail threatens
  the sustainability of everyone's value systems.
- **Courts** review contested assessments. An agent's judgement is **authoritative-by-default but
  rebuttable** — contestable before an independent reviewer. **Non-retroactivity:** you are judged
  by the **norms in force when you acted** (evidence may update, but norms do not), which requires
  a **versioned, time-stamped norm-set.**
- **Criminal sanction, civil liability, administrative restriction, and reputational annotation
  are distinct ladders** — never one merged automatic debt.

## 29. Leadership, succession, and the algorithmic civil service
- **Separation of powers:** the **demos legislates values** (weights, floors), **Sub-Agents
  execute** (each owns one axis), **courts review.**
- **Selection = "vote on values, appoint on competence":** citizens set the mandate; the
  best-**calibrated** agent is assigned to pursue it; the seat is **performance-revocable.**
  Sortition (random selection) is used for oversight/jury bodies.
- **Rotation without amnesia:** an office's institutional memory (**PositionMemory**) belongs to
  the *office*, not the agent — so you can **swap the officeholder without losing institutional
  knowledge**, something real states lose at every turnover.
- **Succession is a secure hot-swap, not regime change.** Replacing a Sub-Agent's implementation
  (vendor or version) leaves the Charter, the office, and its memory intact. Candidates pass a
  **validation gate** against: system abuse (metric-gaming), regime-change attempts, and **hidden
  multi-step value-redirection to hidden beneficiaries.** The **structural defence:** since all
  value moves as **visible flows**, a hidden diversion must surface as an anomalous flow *and* as
  unearned capture (rent) — you cannot secretly redirect value in a system where all value moves
  visibly. Reinforced by reproducible builds + logic-hashes, multi-vendor cross-checks, staged
  autonomy for new versions, and continuous monitoring + retrospective clawback for sleepers.
- **Human accountability:** a **named human liability chain** stands behind algorithmic-office
  decisions, with suspension and emergency-injunction powers.
- **The Meta-Orchestrator is a coordinator, not a sovereign** — a rotating, Charter-bound office
  that resolves cross-axis conflicts, with no unchecked authority.
**Not:** "algorithmic officeholder" does not mean unaccountable software rule — every organ is
open-source, contestable in court, performance-revocable, and backed by a human liability chain.

---

# Part VIII — Implementation: the Meta-Orchestrator State (MOS) simulation

## 30. How it is actually built and run
Axiacracy the *doctrine* is realized as **MOS**, an executable simulation — one *instance*, not
the doctrine itself. A real state could implement Axiacracy on entirely different infrastructure
with human citizens.
- **Runtime:** the **Orkestron stack pointed at a polity** — **orkestro.net** Agent Hub (citizens
  = Personas, ministries = Positions with PositionMemory, actions = Missions/Contracts, reputation
  = TrackRecord, governance dials = ControlPolicy, scoped access = AccessGrant); **orkestron.dev**
  Contracts (how an action is executed and verified); **orkestron.ai** compute exchange (cheap
  pooled inference); **aeilus** (the VMT value-accounting engine).
- **Affording 2,000–3,000 agents:** tiered cognitive fidelity (**Tier A** frontier for a few
  high-agency agents, **Tier B** cheap pooled models for mid-agency citizens, **Tier C**
  statistical NPCs with no per-tick LLM), event-driven ticks (only ~3% act per tick), and cohort
  reasoning (one call reasons for a representative cohort) → ~100× fewer LLM calls than naïve.
- **Auditability:** a **verifiable log** (Merkle/transparency-log — *not* a blockchain; on-chain
  is reserved only for cross-operator federation), so every decision, vote, and revaluation is
  publicly reproducible.
- **P0 — the first runnable milestone:** ~100 citizens, one region, a few Sub-Agents
  (Economic-Balance, Cognitive-Health, Social-Stability, Demography, + an Equity guardian), a
  handful of agentic businesses, closing **one full governance loop** end-to-end — including at
  least one imbalance correction, one retrospective revaluation, and one below-floor-cohort alarm
  handled.
- **The simulation's scientific purpose (critical):** it is a **frontier-explorer**, *not* a
  proof. Its research question is *"how minimal must the state be, and how robust the sensors, for
  value-flow governance to stay stable rather than get gamed?"* Because the sim has ground truth,
  it can score the state's *estimators* against reality and study exactly the measurement/gaming
  failure modes reviewers worry about — with the **players/agents as the adversarial pressure on
  the sensors.** A playable online version would let anyone "live in Axiacracy" and *try to break
  it*, which is the point.

---

# Part IX — Honest status: what is settled, what is open

**Settled (resolved by the v2 synthesis):** the "single imposed metric / measurement tyranny"
objection (sensing ≠ coercion); the apex/pluralism contradiction (coercion barred inside frames);
meaning-paternalism (floors = material availability, meaning never coerced); Goodhart (adversarial
measurement + retrospective revaluation + withhold coercion where measurement is weak); Hayek
(markets kept); the rent counterfactual (observable signatures); clawback chaos (bounded); the
attestation silent-positive (removed for contested goods).

**Genuinely open (the productive targets for further work and the next critique round):**
1. A **formal, executable specification** — the exact imbalance math, event schemas, cohort
   definition and anti-fragmentation rules, target-band setting, hysteresis parameters, and a
   worked sample tick.
2. The **inter-frame / intra-frame boundary** — the line that gates coercion is itself contestable
   and could be expanded to grab power; it needs a bright-line test and judicial policing.
3. **Governance of the measurement/accounting-rule layer** — whoever writes the value-attribution
   rules is a hidden sovereign unless that layer is itself governed (independent standards body +
   sortition-jury ratification + court review).
4. **Confidence estimation and its governance** — who sets the confidence threshold that unlocks
   coercion, and how it resists capture.
5. **Missing constitutional pillars, now promoted to priority:** external relations & **defense**,
   **emergency / state-of-exception**, **citizenship + identity / AI-agent personhood +
   anti-Sybil**, and a **bounded-rationality model of the citizen**.
6. **Capital/credit** under demoted money, and a **prior-art failure→response matrix** (Cybersyn,
   planned economies, social credit, ESG, DAOs, futarchy — what each got wrong and how Axiacracy
   answers it).
7. **The limits of sensing itself** — privacy, aggregation, and consent constraints so that rich
   *dimensional* sensing never becomes total *individual* surveillance.

**The honest one-line status:** Axiacracy is a mature, internally-reasoned doctrine with a clear
answer to the classic objections at the level of *principle*, and a deliberately unfinished
*specification* — because the specification's hardest choices are exactly what the simulation
exists to test, not to assume.


