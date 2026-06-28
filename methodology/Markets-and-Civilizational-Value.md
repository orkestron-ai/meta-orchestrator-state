# Markets & Civilizational Value — reconciling revealed vs deliberative value

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Feeds** | V3 Value Flow, V4 Anti-Value, C1 Business, C2 Market, A7 Incentives, D1 Missions, AIL (A2A) |
| **Created** | 2026-06-28 |

> Resolves a gap: the model had a strong **state↔citizen** loop (deliberative value:
> weights, corridors, sub-agent demand) but omitted the **citizen↔business / A2A market**
> loop (revealed value: citizens direct earned value to suppliers *by demand, not state
> directive*). The two value signals can diverge. This document integrates them without
> (a) recreating central planning, or (b) letting the market override civilizational
> balance.

## The two value signals

| | Revealed value (market) | Deliberative / civilizational value (state) |
|---|---|---|
| Direction | bottom-up, decentralized | top-down, coordinated |
| Signal | where citizens spend earned entitlement | voted weights + corridors + sub-agent demand |
| Strength | local knowledge, preference, speed, allocation/discovery (Hayek) | externalities, long-term, distribution |
| Blind to | externalities, long horizon, concentration | local knowledge, individual preference |
| Axis | mostly `economic` (`$`) | the other 9 axes |

**Two concrete defects of the state-only model:**
1. The state should **not** decide which business deserves reward — that is central
   planning + capture risk. The *citizen's choice* is the reward.
2. **Vote ≠ wallet:** what citizens *vote* as priority (e.g. cognitive health) and what
   they *spend on* (e.g. addictive content) often differ. State-only ignores the market's
   local knowledge; market-only makes orchestration toothless.

This is the article's central tension at the mechanism level: *orchestrate the market, do
not suppress it* ("would not necessarily suppress innovation… balance civilizational
flows").

## Resolution: the market clears, the state prices the residual (multidimensional Pigou)

**Every business↔citizen transaction produces TWO bookings:**

1. **Market booking** (immediate, decentralized): citizen → business, settled on the rail
   (`$`). **The citizen's choice *is* the reward.** The state neither approves nor scores
   it. → fixes defect 1.
2. **Civilizational booking** (deferred, state): the same transaction also yields Æ-deltas
   on *other* axes and anti-value — **the residual the market price missed** (cognitive
   degradation, dependency, ecological, displacement; or positive spillovers: educational,
   scientific, infrastructural). The state does **not** decide "did the business create
   value" (the citizen already did, by spending) — it prices **only the externalities the
   market under-priced.**

This is **Pigou generalized from 1 dimension (`$`) to 10 (Æ):** the state doesn't run the
firm or set its price; it **charges negative externalities and credits positive ones**,
leaving allocation to the market. Crucially it is an **automatic, published, reproducible
function applied uniformly to all flows** — not a per-business political verdict — so there
is no capture and no bureaucracy.

### Three consequences that make this strong
- **Profit ≠ civilizational value (decoupling; reuses orkestro.net BR14).**
  `net_Æ(business) = market_revenue (citizen-directed) − anti_value (state-priced) +
  positive_spillovers (state-credited)`. A profitable-but-harmful BigTech → high `$`, high
  anti-value → low/negative net civ-value → **loses standing/access while still profitable.**
  This mechanizes the article's BigTech-balancing.
- **The vote-vs-spend gap is a first-class diagnostic** (mirror of the claimed-vs-attested
  gap). Don't force deliberative and revealed preference to agree — **measure the
  divergence**; a systematic gap is a signal for a Sub-Agent (e.g. Cognitive Health) to
  reshape the **demand field via incentives, not ban the spend** (Principle 8 + the
  autonomy-vs-paternalism dilemma). Anti-value often hides exactly in this gap.
- **The market is safe to admit because the overlay bounds it.** Concentration self-charges
  (economic ceiling, Principle 7); entitlement is earned multidimensionally + generosity
  multiplier + decay. The market is free to allocate but **cannot run away into
  concentration, because concentration is priced as anti-value.**

## Three coexisting demand sources — one ledger

1. **Citizen private demand** (market, revealed).
2. **State strategic demand** — Civilizational Missions (D1) + Incentives (A7), expressed
   as **market signals** (Æ-credits/subsidies for what's needed), *not* production orders.
   The state is a **large customer with civilizational preferences, not a central planner.**
3. **A2A demand** — folds in with no special case: business at *agent* granularity over the
   **AIL**, carrying provenance so externalities stay attributable.

All three clear through the same Value-Flow ledger.

## What this does to the state↔society coupling
It **moves it to the right layer**, it does not break it. The state↔society loop now
governs the **externality overlay + corridors** (the civilizational layer); **allocation**
is handed to the market. Two complementary loops, not competing ones. The yogurt flow in
`Consumption-and-Settlement.md` is a special case (market booking + reclamation anti-value).

## Guards against state mispricing externalities
- Externality pricing is an **automatic published function** applied uniformly, not a
  per-business decision (removes capture/bureaucracy).
- It is itself **provisional, contestable, revaluable** via the expert + revaluation layer
  (`Governance-Mechanics.md` §B0.3): a mispriced externality can be challenged with
  evidence and re-scored.

## Open decisions for the owner
- **Overlay strength:** how hard does the externality charge bite — light Pigovian nudge
  vs strong corrective? (A dial in E4 ControlPolicy; likely region/era-specific.)
- **Business as agents in P0:** do we stand up a handful of Tier-A *business* agents in the
  P0 region (so the citizen↔business loop is live), or simulate businesses statistically
  first and add agentic businesses in P1?
- **Externality attribution latency:** how long after a transaction can the civilizational
  booking still attach anti-value (ties to the detection-lag question in the anti-value
  block).
