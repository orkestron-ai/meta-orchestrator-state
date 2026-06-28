# Value ↔ Money Coupling — instant enforcement + retrospective clawback

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Feeds** | V3 Value Flow, V4 Anti-Value, A8 Treasury, E4 ControlPolicy, B4/quality-TrackRecord; reuses orkestro.net AccessGrant + ControlPolicy trust-ramp |
| **Created** | 2026-06-28 |

> The disease of the real world: **anti-value and money live in separate systems** —
> money clears instantly in markets, harm is accounted later through a political chain
> (discontent → politicians → laws → antitrust agency → redistribution). All the delay
> lives in that gap, and in it a business gets rich and makes society miserable before any
> consequence lands.
>
> **The MOS move: put anti-value and money in the *same ledger*, cleared in the *same
> tick*.** The coupling becomes automatic and instant — the political transmission belt is
> replaced by an accounting invariant.

## "I lose money in the form of what — fines?" → No. Five automatic mechanics.

A fine is a punitive, after-the-fact, discretionary decision by an official: slow,
gameable, capturable. MOS replaces it with **five automatic ledger mechanics**, no
per-case human decision:

| # | Mechanic | What it does |
|---|----------|--------------|
| 1 | **Externality-escrow** | a fraction of every business inflow is withheld, sized by *exposure* = `sector_profile × (1 / quality_TrackRecord)`. **You cannot bank revenue whose externalities have not yet settled.** Kills the root real-world problem (enrich before harm is accounted). |
| 2 | **Continuous anti-value debit** | anti-value is debited from standing **and** escrow **in the same tick** it's earned. No law written per case — the accounting *is* the law (public, reproducible function). |
| 3 | **Concentration charge** | above the economic ceiling, marginal accumulation is discounted/charged continuously (Principle 7). No runaway wealth without a rising charge. |
| 4 | **Standing / access loss** | quality-TrackRecord gates draw-rights, scarce inputs, and the escrow ratio itself (trust-ramp). Anti-value rises → escrow auto-tightens. The "antitrust agency" becomes a continuous dial, not a separate body. |
| 5 | **Retrospective clawback** | for what was missed — see §3. |

## 1. Two halves: prevention (instant) + correction (retrospective)

- **Prevention** = escrow + ceiling + continuous debit + trust-ramp. Acts *now*, on
  detectable-at-transaction externalities.
- **Correction** = revaluation + clawback. Acts *later*, on latent/concealed harm.

## 2. The instant loop (per tick, per business)

1. **Revenue inflow** (market booking) → split: part to liquid balance, part to
   **externality-escrow** sized by exposure.
2. **Externality residual measured** (V4) → **anti-value charge booked same tick** →
   debits standing + escrow.
3. **Concentration above ceiling** → continuous concentration charge.
4. **Escrow releases** as externality windows close with no materialized harm; **forfeits
   to remediation** if harm materializes.

### Why this is instantaneous — the real chain, collapsed
| Real world | MOS |
|---|---|
| harm → public discontent | harm is **measured** (sense, V4), not inferred from discontent |
| → politicians → laws | **automatic function**, no per-case legislation |
| → antitrust agency | continuous escrow/ceiling dial (Economic Balance Sub-Agent) |
| → redistribution (years) | debit in the **same ledger, same tick** |

**Honest boundary.** "Instant" applies only to externalities *detectable at transaction
time*. Latent harms (dependency, meaning-loss, concentration) surface later — held by
escrow + caught by retrospection.

## 3. The retrospective loop (triggered, not per-tick)

1. **Retrospective analysis / petition** surfaces under-priced past harm.
2. **Revaluation** reopens the *settled* flows, re-prices the externality with new evidence
   (expert-calibrated, `Governance-Mechanics.md` §B0.3).
3. If the harm is of the **clawback-eligible class** (see §4) → **clawback against the
   business's accumulated assets.**
4. Clawed value is **earmarked to remediation of exactly the cohorts/dimensions harmed**
   (displaced workers, degraded-cognition cohort, damaged ecology) — *not* a general,
   opaque treasury — and is fully traceable. ("Their gains close the problems they made.")

## 4. Clawback vs legal certainty (the dilemma, resolved)

If anything can be re-priced forever, business cannot plan and no one invests; real law
uses statutes of limitation for exactly this. Principled line, by analogy with how law
treats **fraud** differently from honest error:

- **Finality for the honest:** ordinary value settles and is final → predictability.
- **Perpetual liability for the concealing:** **systemic anti-value that was concealed or
  is grossly large** stays **clawback-eligible indefinitely.** Honest-but-mistaken value is
  safe; concealed/gross accumulation is never safe.

This balances correction against the stability / investment-certainty dilemma.

## 5. Guard against the charge becoming a capture weapon
Mispricing an externality is itself harmful (it could be weaponized against a rival). So
the charge is: an **automatic function applied uniformly** (no per-business discretion) +
**provisional, contestable, revaluable** (the same revaluation machinery cuts both ways) +
**expert-calibrated** with on-ledger conflict-of-interest. The enforcer is the ledger, not
an official.

## Coupling primitives (for V4 / A8 / E4)
- `externality_escrow` — withheld inflow fraction; released on clean settlement, forfeited
  to remediation on materialized harm.
- `anti_value_charge` — Æ debit at flow time (provisional) and at revaluation.
- `concentration_charge` — continuous charge above economic ceiling.
- `clawback` — retrospective debit vs accumulated assets; eligible class = concealed/gross
  systemic anti-value.
- `remediation_routing` — charged/clawed value earmarked + traced to the measured-harmed
  cohorts/dimensions.
- `exposure` / escrow-ratio + trust-ramp — reuses orkestro.net AccessGrant + ControlPolicy.

## Open knobs for the owner
- Escrow fraction curve vs exposure; ceiling level per region/era.
- "Gross magnitude" threshold and the concealment test that flips a flow into the
  perpetual-clawback class.
- Remediation routing: direct-to-cohort vs via a Sub-Agent-run program (A7).
