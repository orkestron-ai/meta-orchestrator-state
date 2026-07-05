# Relative Value & Inter-Frame Routing — value across heterogeneous units and frames

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Grounds** | VMT T13 (no universal optimum), A12 (no conservation), A13 (partial commensurability), A6 (realization at consumption), A4 (plan≠fact), A10 (inter-system via external flows), T12 (autocatalysis), T7 (participation) |
| **Builds on** | `Value-Frames-and-Perspectival-Value.md`, `Markets-and-Civilizational-Value.md`, `Value-Money-Coupling.md` |
| **Created** | 2026-06-28 |

> Two questions, one root — **how to handle value when there is no single ruler**:
> (1) different currencies/prices across regions — how is the "balance" set, and is it even
> about *fairness*? (2) how are non-state value systems connected to the state's, why
> measure them in the Æilus ledger, and how does that connect to money flows?

---

## Part 1 — Relative value without a universal unit

### There is no absolute "fair" ratio — reframe fairness → sustainability
VMT is explicit: **no universal optimality criterion (T13)**, **no conservation of value
(A12)**, **only partial commensurability (A13)**. A "fair absolute price" is a category
error. So the criterion is not *fair* but **"sustainably moves the system toward the state
frame's targets."** (The owner's hunch — "maybe it's not about fairness" — is correct.)

### Two separations that dissolve the currency/price problem
1. **Intra-axis (substitutable goods: apple vs bread)** → ratios are **discovered by the
   market** from revealed demand. The state does **not** set them (Hayek's calculation
   problem). Here market "value discovery" (the Austrian *axiocracy*) is a working
   sub-mechanism.
2. **Inter-axis (economy vs ecology vs meaning)** → set by the **voted weights `w(t)`** —
   the *state frame's* relative valuation across axes. **This** is the only "balance" the
   state sets; it never sets intra-market prices.

### Across currencies, the invariant is Realized Æ, not price
By **A6**, value is realized at consumption as a **change in the receiver's state**. A loaf
that relieves hunger books ~the same realized nutritional/wellbeing Æ whether it settled for
1 or 100 units of local currency. Therefore:

- **Do not convert currencies at the value layer.** Currency/price is a **local settlement
  rail** that floats freely; the **invariant is Realized Æ** (currency-independent).
- Compare **realized value**, not nominal price — a generalized PPP in Æ-space. If a
  numéraire is needed, use a **reference basket of flows** (an SDR analogue), not money.
- "Different currencies" is a *symptom of forcing a universal scalar*. In vector Æ-space no
  universal equivalent is needed — and by **T1** none truly exists; money only *pretends*
  to be one by flattening all value onto one axis.

### Honest ratios are computed, not decreed
When nominal price diverges from realized value, that gap **is** Flow Resistance / Leakage
(Planned≠Realized, T4/A11) → an anti-value signal. Manipulated prices surface themselves,
continuously.

### The real objective
**Maximize the state frame's civilizational value, subject to constraints: per-cohort
floors + participation conditions θ.** Fairness enters as **constraints that keep the
optimization sustainable**, not as the objective function.

---

## Part 2 — Why measure other frames; the state as inter-frame router

**The lever:** knowing an actor's value system (what is valuable *to them*) lets the state
**pay them in the currency of their own frame** — far cheaper and more motivating than money.

### Three payoffs

**(a) Targeted incentives in the actor's own currency — positive-sum, value-creating.**
Knowing money only → the state pays money (blunt, expensive). Knowing that a scientist most
values *a hard problem + recognition* (≈free to the state), a parent *time/flexibility* → it
gives **that**. The incentive's *planned* value (state frame) is low-cost; its *realized*
value (actor frame) is high; the gap is **positive — value is created** (A12, A4, A13), not
transferred.

**(b) Participation-condition monitoring.** Measuring an actor's frame reveals their **θ** —
when a valuable company/person is about to disengage / exit / change form (T7), and **why** —
early enough to act. The owner's example (a super-valuable company) is (a)+(b): the state
invests in what *they* value (cheap when frames match well) → they stay and produce more →
an **autocatalytic loop (T12)**.

**(c) The state as a value router / matchmaker across frames.** Knowing many frames, the
Æilus ledger finds **positive-sum exchanges the actors can't see and money-markets miss**
(markets match only on the economic axis; this matches on the full Æ-vector). Company values
talent + university values funding + citizen values meaning → the ledger composes a
three-way flow (company funds a research chair, gains a talent pipeline, citizen gets
meaningful work) no money-market would assemble. The state is a **market-maker / flow-router
in value-space** — a **catalyst, not an owner** (consistent with "no apex"). The mega-graph
of frames is not something that "converges to the state"; it is the **substrate for
matchmaking**, where the state adds value by *revealing and enabling* latent flows (a Flow
Owner reducing network resistance).

### The connection to money flows
Frame-knowledge makes money flows **smaller and better-aimed**. The state either
(i) **subsidizes exactly what the actor values** (a targeted Pigouvian credit instead of
generic cash), or (ii) **substitutes non-money value for money** (recognition, autonomy,
mission — ≈0 money, high realized Æ). **The richer the population's value frames (valuing
non-money goods), the less money the state must circulate** — a direct bridge to the
article's money→value-civilization thesis. Conversely, an actor whose frame values *only
money* forces the state to spend money. Money is used only where it is the cheapest rail.

### Guardrails (without these, this is a manipulation / surveillance engine)
- **Boundary-only (A10).** The state sees only what an actor **publishes/attests** to the
  shared ledger — never the internal graph of a family/psyche. No god's-eye view.
- **Serve a frame, don't rewrite it.** The state may *give you what you value* (a transparent
  incentive you accept or decline); it may **not engineer your preferences**. Incentive vs
  propaganda = transparency + consent + serves the actor's own goals (Principle 12).
- **Anti-concentration still binds.** Investing in a strong actor is capped by the
  concentration ceiling and must not push others below floor; the generosity multiplier
  rewards passing received value on.
- **Exit / θ is the check.** If it is coercive, θ is violated and the actor exits (T7). The
  right to exit disciplines the state.

## Part 3 — Privacy-preserving frame disclosure (how the state learns a frame without reading the ledger)

The state must learn the **shape** of an actor's frame without the **raw ledger**. Design:

- **A scoped access grant** (reuse orkestro.net AccessGrant: scoped, time-limited) yields
  **not transactions but a derived frame summary** — axis-weights + top value-categories,
  computed from the actor's **highest realized/given flows** (what delivered them the most
  value per unit given → their strongest preferences). The **raw flows never cross the
  boundary** (A10 — only a *projection* does).
- **Computed locally by the actor's own agent, published at a granularity the actor
  chooses.** More disclosure → better-targeted incentives *for them* (an opt-in benefit);
  less → more privacy. This is the actor's dial (the "serve, not surveil" guardrail).
- **Default = cohort aggregates only** (differential privacy / k-anonymity), individuals
  non-identifiable. **Individual disclosure is opt-in**, justified by the personalized
  benefit (targeted incentives, matchmaking).
- **Zero-knowledge / attestation:** an actor can *prove* a frame property ("I value
  education highly") without revealing the underlying transactions.

Net: the state sees the **form** of the frame, never the **contents** of the ledger.

## Open knobs for the owner
- Frame-summary granularity levels and the exact "top realized/given" extraction function.
- Matchmaking scope in P0: pairwise only, or multi-party value composition?
- The reference basket (numéraire) definition for cross-region realized-Æ comparison.
- Limits on state incentive-targeting to keep it "serve, not shape" (audit of incentives).
