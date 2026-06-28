# Consumption & Settlement — how citizens spend earned value

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Feeds** | V3 Value Flow (settlement semantics), V4 Anti-Value (reclamations), B4 standing, C2 Market |
| **Created** | 2026-06-28 |

> Answers: *how do I take a yogurt off the shelf using earned value, have the state book
> the planned consumed value, raise a reclamation if it's spoiled (business charged
> anti-value for my poisoning) — without drowning in bureaucracy, and without money's
> distortions?*

## The core move: money conflates three things — separate them

| Concern | Money's behaviour | MOS |
|---|---|---|
| **Entitlement** (what I may draw from the commons) | = prior `$` income only | earned by **multidimensional** contribution (B4 standing → draw-rights) |
| **Settlement** (transfer + record of the good) | instant bearer transfer | thin settlement rail (may be `$`), low-ceremony |
| **Quality attestation** (did it deliver?) | externalized (warranty law, courts, reviews) | **first-class**: realized-value gap auto-charges anti-value |

The quagmire appears only if you try to run *settlement* through the *sovereign* layer.
So: **two layers, clean separation.**

- **Sovereign layer = the Æ-ledger** — multidimensional value accounting, non-transferable;
  holds entitlement and anti-value.
- **Convenience layer = a settlement rail** (can be `$`) — fast, impersonal, low-ceremony.
  `$` stays **one Æ axis + a settlement instrument, NOT the steering variable.**

The two failure modes to avoid: sovereign-runs-settlement (bureaucratic quagmire) **or**
settlement-is-sovereign (money's distortions return).

## Three mechanisms that kill the bureaucracy

### 1. Ceremony proportional to stakes (mirrors the cognitive tiers A/B/C)
| Tier | What | Ceremony |
|---|---|---|
| **T0 ambient** | yogurt, routine, low stakes | checkout records *what was taken* + its planned value-cost. Auto-record, auto-settle. **Silence = attestation.** |
| **T1 attested** | a service, course, repair | lightweight beneficiary attestation (score / thumbs) |
| **T2 reviewed** | high-stakes / disputed / sampled audit | full independent review + possible revaluation |

Heavy machinery fires **only at T2**.

### 2. Default-trust; reclamation by exception
The good is assumed to deliver its standard value; the provisional flow **auto-settles**
after a short window **unless contested**. You do not attest every yogurt. Spoiled →
`ValueDisputed` (reclamation): business charged anti-value proportional to harm (mild =
refund; poisoning = large charge on `health`/`social_stability` + escalation), citizen
refunded. **False reclamation costs the claimant's TrackRecord** (like over-claiming) →
self-policing without per-item bureaucracy.

### 3. Statistical QC instead of universal review
The system audits a **sample** of a business's flows and watches **aggregate reclamation
rate** → rising spoilage = **systemic anti-value**, forming the business's *quality
TrackRecord* (gates access to scarce inputs). Reputation does, continuously and cheaply,
what warranty bureaucracy does today.

## Why the *simulation* structurally dodges the bureaucracy cost
Real-world "bureaucracy" is the cost of **human attention**. In MOS, **recording a
transaction is free** (it's data, not paperwork); attention (LLM calls) is spent only on
**judgment**, and judgment is bounded by the cognitive tiers. The quagmire is a
human-attention problem the model avoids everywhere except T2.

## Honest verdict on money
Money is unbeaten at exactly one job: **low-ceremony, impersonal settlement of routine,
voluntary exchange.** So MOS does not discard it — it **demotes it from sovereign to
instrument.** `$` = a settlement rail + one axis; the Æ-ledger is sovereign. What MOS adds
on top of money: (a) the claimed-vs-realized value gap is first-class (reclamations
auto-charge anti-value); (b) entitlement is earned by multidimensional contribution (a
scientist/parent/mentor accrues draw-rights with no market wage); (c) externalities are
priced. Consistent with the article: *"money does not disappear — `$` remains one axis."*

## Yogurt, end to end
1. `DrawMade` — checkout books a **provisional** Value Flow: business → citizen
   (+nutritional/economic Æ to citizen, −entitlement, +economic Æ to business), planned
   value-cost from a public catalog. Zero ceremony.
2. **No complaint within window** → auto-`settled`. Done.
3. **Spoiled** → `ValueDisputed` → realized-value gap booked; business `anti_value`
   charge (scope=edge; if pattern across many citizens → systemic) + citizen refund;
   business quality-TrackRecord updated. Heavy path, but only here.

## Feeds P0
Minimum new fields/objects: citizen **entitlement balance / draw-rate**, public
**value-cost catalog**, `DrawMade` event, `ValueDisputed` (reclamation) event, business
**quality-TrackRecord**.

## Open decision (gates anti-value work)
**Recommended:** adopt the two-layer model — `$` demoted to settlement rail + one axis,
Æ-ledger sovereign. Anti-value pricing in `Value-Axes…`/the anti-value piece assumes
this. Alternative (pure value, no money rail) is cleaner conceptually but reintroduces the
per-transaction ceremony cost at T0. **Confirm before the anti-value block.**
