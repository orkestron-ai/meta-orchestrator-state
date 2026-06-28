# Courts & Adjudication — interpretable value, contestable, judged by contemporaneous norms

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Feeds** | A6 Judiciary, V4 Anti-Value, A1 Constitution, E2/verifiable-log (versioned norms) |
| **Reuses** | orkestro.net Review (reviewer-independent BR2; rework ≤ 3 → escalate BR4) |
| **Created** | 2026-06-28 |

> Value and anti-value are **interpretable** quantities. State agents are allowed an
> authoritative view that everyone trusts — but any anti-value declaration must be
> **contestable in court**. And courts must judge on the **value-frame (weights, corridors,
> pricing function) that was in force *at the time of the act*** under investigation, not
> today's.

## 1. Interpretive authority is rebuttable, not infallible

A Sub-Agent's value / anti-value assessment is **authoritative-by-default but appealable**
(a rebuttable presumption). Its weight comes from **transparency, not infallibility**:
public logic (commit-hash referenced), an on-ledger calibration TrackRecord, disclosed
conflicts of interest. An affected party can appeal.

An anti-value declaration is therefore just another **claim** in the
`provisional → attested → settled → revalued` lifecycle, and the **court is the T2 review
authority** for contested ones. It reuses the judiciary pattern (A6): reviewer independent
of the declaring agent (BR2), bounded rework then escalation (BR4). The court can uphold,
adjust, or reverse the charge.

Courts are themselves accountable: judges are Tier-A agents with calibration / TrackRecord;
rulings are appealable and escalate to the constitutional level. **There is no final,
unaccountable authority — only escalation bounded by the constitution.**

## 2. Non-retroactivity — judge by the norms in force at the time of the act

The value-flow analogue of *nulla poena sine lege* / no ex-post-facto law (ICCPR Art. 15):
**judgment applies the norm-set binding when the act was committed, never the present one.**
You cannot charge anti-value for violating weights/policies that did not exist when the
actor acted.

### The reconciliation with revaluation
This seems to collide with the **revaluation** mechanism (re-pricing past flows when new
harm surfaces). It does not, once two things are separated:

| What can change | Retroactive? | Why |
|---|---|---|
| **Evidence / facts** about consequences | **Yes** — updatable | we legitimately *learn* what actually happened (the yogurt poisoned; the content created dependency) |
| **Norms** (weights `w(t)`, corridors, pricing function) | **No** — frozen at act-time | norms are the *law*; judging by future norms is ex-post-facto |

→ **Revaluation re-prices using NEW EVIDENCE but the CONTEMPORANEOUS NORM-SET.** The actor
is not sandbagged by future moral fashion (rule of law), yet does not escape the real
consequences of the act (accountability).

### Why the concealment / clawback exception stays consistent
The perpetual-clawback class (`Value-Money-Coupling.md` §4) is **concealed or gross**
systemic anti-value. **Concealment violated the *contemporaneous* norms too** (hiding harm
was already wrong) — so perpetual liability is *not* retroactive norm-application; it
enforces an old norm whose breach was merely discovered late.

## 3. What this requires — a versioned, time-indexed norm-set

Every governing norm is recorded on the verifiable log with a **validity interval**:
- the weight vector `w(t)` of every voting round,
- every corridor (floor / target_band / ceiling) version,
- every externality **pricing-function** version (by commit-hash).

Courts and revaluation query: *"what norm-set was binding at time T?"* Our transparency
design (reproducible tally + commit-hash citations) already supports this; we only make
**norm-versions first-class and time-indexed.**

## 4. Adjudication flow (a contested anti-value charge)

1. Sub-Agent books a **provisional** anti-value charge (its interpretation).
2. Affected party **appeals** → opens a case (A6).
3. Court assembles: (a) the **contemporaneous norm-set** at act-time, (b) the **evidence**
   (incl. any new facts), (c) an **independent reviewer** (≠ the declaring agent, BR2).
4. Ruling: uphold / adjust / reverse → the charge moves to `settled` or is voided.
5. Bounded rework (≤ 3) → escalate to a higher court / constitutional level (BR4).
6. The whole case is on the verifiable log — public, reproducible.

## 5. New constitutional principles (add to `Governance-Mechanics.md` A0)

- **Principle 14 — Non-retroactivity / contemporaneous judgment.** Acts are judged by the
  norm-set in force when they were committed. Evidence updates retroactively; norms do not.
- **Principle 15 — Interpretive authority is rebuttable.** Every value / anti-value
  assessment is authoritative-by-default but contestable in court; trust derives from
  transparency and calibration, not infallibility; no final unaccountable authority.

## Open knobs for the owner
- Court composition in the simulation: a single Judiciary Sub-Agent vs an elder/peer panel.
- Standard of proof for reversing an agent's charge (and for the concealment test).
- Appeal-window length and how it interacts with the escrow-release window.
