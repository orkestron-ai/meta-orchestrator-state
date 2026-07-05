# Open Decisions — consolidated checklist before P0

| | |
|---|---|
| **Status** | **DRAFT — awaiting owner ratification** |
| **Purpose** | One pass over every open knob scattered across the 10 methodology docs, split into: **LOCKED** (already decided), **GATE** (must decide to assemble P0), **PARAM** (default now, calibrate in sim), **DEFER** (external / later phase). |
| **Created** | 2026-06-28 |

> **How to use:** you only need to actively decide the **GATE** items. **PARAM** items have
> sensible defaults proposed — accept wholesale or override individual ones. **LOCKED** is
> for the record. **DEFER** is explicitly out of P0.

---

## LOCKED — already decided (for the record)

| # | Decision | Source |
|---|----------|--------|
| L1 | Govern by value-flow balancing, not taxation; money demoted to instrument + one axis | Charter Art. 1, 13 |
| L2 | Tier-A cognitive share = a **simulation dial (10–90%)** | Governance Q3 |
| L3 | **Single region** for P0; `region` + `cohort` first-class from day one | Governance Q4 |
| L4 | **Verifiable log now**, on-chain optional for federation (deliberate simplification) | Governance Q6 |
| L5 | **Liquid democracy**: individual voting + revocable topic-scoped party delegation + concentration caps | Governance Q7 |
| L6 | **Lightweight frames** in P0 (per-actor weight vector + θ), full `ValueSystem {A,F,G,R,T}` in P1 | Frames; owner 2026-06-28 |
| L7 | **Charter extracted** as the supreme document; A0 principles are its source | owner 2026-06-28 |
| L8 | Repo split methodology / implementation / source; in git (`orkestron-ai/meta-orchestrator-state`) | owner |
| L9 | Working doctrine name **Axiacracy** (domain `axiacra.cy` ordered) — **rebrand deferred until registrar confirms** | owner |

---

## GATE — decisions that gate P0 design (need your call now)

Each: the decision · options · **my recommendation** · what it affects.

**GATE-1 — Final axis set & the 10th axis.**
Adopt all **10 axes** as the shared vocabulary; confirm **`epistemic` as its own axis** (vs folding into `cognitive`).
→ **Rec: 10 axes, `epistemic` standalone** (anti-propaganda is now central). Affects V2, voting, every Sub-Agent.

**GATE-2 — Which axes are *instrumented* in P0.**
You can't meaningfully exercise all 10 with ~100 citizens. Pick the P0-active subset.
→ **Rec: 5 —** `economic`, `cognitive`, `social_stability`, `meaning`, `demographic`. (Richest value/anti-value dynamics; the rest stay in the vocabulary, inert.) Affects Sub-Agent choice, activity catalogue, floors.

**GATE-3 — Which State Sub-Agents in P0.**
Each owns an axis and runs sense→diagnose→demand.
→ **Rec: 4 —** Economic Balance, Cognitive Health, Social Stability, Demography (+ an **Equity/Ombudsman guardian** folded in, watching cohort variance & floors). Affects E1/E3, the loop.

**GATE-4 — Which frames are first-class in P0.**
→ **Rec: citizen + state + 2–3 Tier-A business agents.** Family = P1. Business must be live so the citizen↔business market loop (revealed value + externality overlay) actually runs. Affects Markets loop, C1/C2/C5.

**GATE-5 — Business: agentic or statistical in P0.**
→ **Rec: 2–3 Tier-A *agentic* businesses** (enough to exercise market booking + externality residual + one anti-value profile), rest statistical. Affects the whole market/Pigou demonstration.

**GATE-6 — Lock the two-layer money model.**
Formally ratify: sovereign Æ-ledger + thin `$` settlement rail; realized Æ is the cross-frame invariant.
→ **Rec: lock it.** It underpins consumption, markets, value-money coupling, relative-value. (Operating on it already; just needs an explicit yes.)

**GATE-7 — P0 dispute/revaluation path.**
Full judiciary (A6) is P1, but P0 needs *some* contestation to test the value lifecycle.
→ **Rec: a lightweight single-independent-reviewer path** in P0 (reviewer ≠ declaring agent) that can run **one revaluation** end-to-end; full courts/constitutional-review panel = P1. Affects the P0 success criteria.

**GATE-8 — P0 success criteria (what "closing the loop" means).**
→ **Rec:** one full governance tick-cycle (act → book value → sense imbalance → generate demand → incentivize → re-sense) **+ at least one imbalance correction + one revaluation + one below-floor cohort alarm handled.** Affects what we build first.

---

## PARAM — default now, calibrate in simulation (do NOT block P0)

Accept the defaults wholesale or override individually.

| # | Parameter | Proposed P0 default | Source |
|---|-----------|--------------------|--------|
| P-1 | `v_max` vote cap · quadratic curvature · party-discount threshold | v_max = 3× median reputation; quadratic cost `k²`; party discount above 20% delegated weight | Axes |
| P-2 | Per-axis initial floors / target_bands (normalized 0–100) | floor 30 · band 45–70 · ceiling 90 for each P0 axis; tune per axis after first run | Axes |
| P-3 | Voting cadence · delegation granularity | per **sim-week**, + imbalance-triggered emergency vote; delegation per-axis | Axes |
| P-4 | Externality **overlay strength** (Pigou bite) | **moderate**; an E4 dial, region/era-specific | Markets |
| P-5 | Externality attribution latency in P0 | **short window only** (long-lag/clawback deferred to P1) | Markets/Anti-Value |
| P-6 | Escrow fraction curve · ceiling level | escrow = 10–30% scaled by exposure; ceiling per P-2 | Value-Money |
| P-7 | Responsibility-share attribution | **proportional-exposure only** in P0 (Shapley-approx = P1) | Anti-Value |
| P-8 | Systemic-harm baseline/counterfactual | **rolling baseline** (trailing window) | Anti-Value |
| P-9 | Lag thresholds per axis · escrow hold = f(lag) | default lag table; escrow hold = min(lag, cap) | Anti-Value |
| P-10 | Intent/kind determination | **explicit tags** on modelled activities (sim has ground truth); inference = later research | Charter-Rights |
| P-11 | Inviolable-rights core | life, bodily integrity, liberty, consent, exit | Charter-Rights |
| P-12 | Remediation routing | **direct-to-cohort** in P0 (A7 program = P1) | Value-Money |
| P-13 | Concealment / "gross" threshold + test | placeholder heuristic; refine with clawback in P1 | Value-Money/Courts |
| P-14 | θ estimation | compute θ from **ground truth** in P0; test **boundary-only estimator** as a research metric later | Frames |
| P-15 | Frame-summary granularity + extraction | coarse top-k value categories (C6 routing = P2) | Relative-Value |

---

## DEFER — explicitly out of P0

| # | Item | Why deferred |
|---|------|--------------|
| DEF-1 | **ELMM tie-in** (MOS as ELMM instance vs own Dimension) | owner will send context; provisional = own Dimension; doesn't block P0 |
| DEF-2 | **C6 Inter-Frame Routing / matchmaking** (pairwise vs multi-party; reference basket) | P2 capability; not needed to close the P0 loop |
| DEF-3 | **Retrospective clawback machinery** (full) | P1 (long-lag harms); P0 tests short-lag + one revaluation only |
| DEF-4 | **Full judiciary / constitutional-review panel** | P1; P0 uses the lightweight path (GATE-7) |
| DEF-5 | **Parties, Experts, Recognition** (B7/B8/B9) as live agents | P1; P0 voting is direct, no delegation needed at 100 citizens |
| DEF-6 | **Family frame** (B3) | P1; P0 frames = citizen + state + business |
| DEF-7 | **Rebranding** to Axiacracy across repo | pending domain confirmation |
| DEF-8 | **Incentive-targeting "serve-not-shape" audit** | P1 guardrail; note only in P0 |

---

## Next step
On your ratification of the **GATE** block (and any **PARAM** overrides), the P0 assembly
can proceed cleanly: Namespaces V1–V5 + fields, the citizen activity catalogue
(value / anti-value), the P0-active axes/Sub-Agents, and the closed governance loop.
