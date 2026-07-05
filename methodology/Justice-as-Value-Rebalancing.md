# Justice as Value Rebalancing — the court as a rebalancing operator over harmful events

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Extends** | `Courts-and-Adjudication.md`, `Anti-Value-Taxonomy.md`, `Value-Money-Coupling.md` (remediation routing), and the judicial section of `Ministries-Branches-and-Municipality.md`. |
| **Idea** | Every event/action is a **change of state in the value flows.** The judiciary is not a separate punitive institution — it is the **operator that measures a harmful event, restores those it harmed across every damaged axis, and applies a commensurate deterrent, rebalancing the graph.** |
| **Created** | 2026-06-28 |

---

## 1. The reframe: an event is a value-flow state-change
Anything that happens — a sale, a service, a contribution, a harm — is a **movement of value /
anti-value elements** in the graph. The system **provisionally books** it as it happens (this is
*sensing*, not punishment), and evaluates it against the **thresholds** on the affected axes. When a
harmful event **crosses a threshold**, it enters the judicial pipeline, whose output is a
**commensurate response that rebalances** the graph. Justice is therefore *value-native and
computational*, not the application of an arbitrary sentence.

## 2. The pipeline (event → response)
1. **Sense & provisionally book** the event (the anti-value flow) — immediate, on the verifiable log.
2. **Measure** four things: the **magnitude** of anti-value **per axis**; the **affected set** (every
   transformer on the receiving end of the harmful flow — read from the flow record, *not* just the
   complainant); the **intent/kind** (negligent / malicious / concealed); and **which threshold** was
   crossed.
3. **Adjudicate** (due process): establish **causation** and **magnitude**, with the accused's **right
   to contest** (was it my product? was the harm mine? was I negligent?), judged by the **thresholds in
   force at the time of the act** (non-retroactivity). *"Immediate" applies to the booking; the*
   ***response*** *is adjudicated, never summary.*
4. **Order the commensurate response** = **restoration + deterrence** (§3).
5. **Route & rebalance** — restitution flows to exactly those harmed (remediation routing); the actor's
   standing/escrow is debited; re-sense.

## 3. The response = restoration (primary) + deterrence (secondary)
```
response = restore( affected_set , damage_per_axis )        ← make every harmed party whole, per axis
         + deter( anti_value_magnitude , intent/kind , recurrence )   ← proportional, escalating penalty
```
- **Restoration is primary and multidimensional.** Each **damaged axis** is restored to each
  **damaged party**: economic loss → refund; bodily harm → treatment cost; psychological/moral harm →
  moral damages (on the meaning/wellbeing axis). The harm was on several axes, so the remedy covers
  all of them.
- **Cohort restitution without every victim suing.** Because the ledger records who received the
  harmful flow, the court restores the **whole affected set** (all buyers), not only the complainant —
  proactively. (This is the inverse of a "claimant industry": restitution is *computed from measured
  harm to the actual affected set*, not claimed by opportunists.)
- **Deterrence is secondary and escalating.** Above restoration, a penalty **proportional to the
  anti-value magnitude**, scaled by **intent** (negligent < malicious < concealed) and **recurrence**
  (the exponential escalator), applied along the escalation ladder (annotation → charge → restriction →
  loss of liberty). Restoration makes victims whole; deterrence prices the externality and prevents
  recurrence.
- **Irreversible harm** (death, permanent injury) — restoration is impossible, so: the **criminal
  ladder** (incapacitation justified by A9 — a participant who makes others' θ fail), **maximal
  restitution to dependents**, and the harm **booked as permanent anti-value**.

## 4. Worked example — the expired yogurt (the owner's case, fully)
1. **Event & booking:** a business sells expired yogurt; a buyer reports poisoning → a
   `ValueDisputed` anti-value event is booked provisionally.
2. **Measure:** the court reads the **flow record** → the **affected set = every buyer of that batch**
   (not just the complainant). Per-axis damage: **economic** (purchase price), **health** (treatment
   cost), **meaning/psychological** (moral damage). **Intent:** was the expiry **negligent** (missed) or
   **concealed** (knowingly sold)? **Threshold:** the poisoning crossed a **bodily-harm** threshold.
3. **Adjudicate:** establish causation (did *this* product cause the illness?) and magnitude, with the
   business's **right to contest**, judged by the health-harm thresholds **in force at the time of
   sale**.
4. **Commensurate response:**
   - **Restore** — **refund all buyers** of the batch (economic); **pay treatment** for those harmed
     (health); **pay bounded moral damages** for the poisoning (meaning/psych).
   - **Deter** — a penalty scaled by magnitude × intent (higher if the expiry was **concealed** →
     toward the criminal ladder) × recurrence.
   - **Route** — restitution to the harmed set; the business's **escrow forfeits**, its **quality
     standing drops**, and if concealment is found it faces **clawback + the criminal ladder**.
5. **Rebalance & re-sense** — the graph is restored; the business's record reflects it.

## 5. Key properties
- **Restorative-first**, not merely punitive — the default output makes the harmed whole.
- **Multidimensional** — every damaged axis is restored to whoever it was damaged on.
- **Cohort-wide by computation** — the affected set comes from the flow record, so victims need not
  individually litigate.
- **Commensurate & escalating** — proportional to measured magnitude, intent, and recurrence.
- **Due-process-preserved** — immediate *booking*, **adjudicated** response; the accused may contest
  causation and magnitude; judged by contemporaneous norms.
- **Confidence-graded (honest limit):** economic and medical restitution are **high-confidence**
  (objective) → firm awards. **Moral/psychological** damage is **low-confidence** (subjective) → use
  **bounded schedules/tables**, never open-ended awards — keeping it consistent with "coerce only on
  defensible measurement" and blocking a claimant industry.

## 6. What this unifies
It fuses the **T2 review tier** (`Consumption-and-Settlement.md`), the **A6 judiciary**
(`Courts-and-Adjudication.md`), **remediation routing** (`Value-Money-Coupling.md`), and the
**escalation ladders** into one coherent operator: *measure the harmful event → restore across axes →
deter proportionally → rebalance.* The court is where the value substrate's accounting becomes lived
justice.

## Open items
- The **causation standard** and burden of proof per harm class (esp. for long-lag/systemic harm where
  causation is statistical, not direct).
- The **moral-damage schedule** (bounded tables per harm class and axis).
- The **affected-set privacy bound** — using transaction records to identify all buyers is a
  proportionate, warranted use (§0 apparatus), but its limits need a bright line.
- Handling **systemic** harm (content dependency) in this frame: the "event" is a *pattern*, the
  affected set a *cohort*, restitution *statistical* — a harder case than the edge-harm yogurt.
