# Axiacracy vs. MOS — the boundary between the doctrine and one realization

| | |
|---|---|
| **Status** | **DRAFT v0.1 — the separation** |
| **Purpose** | Draw the explicit line between **Axiacracy** (the universal, deployment-agnostic doctrine — *the invariants any instance must satisfy*) and **MOS** (the Meta-Orchestrator State — *one concrete realization*, with its own free choices). We deliberately went deep into MOS to *find these boundaries*; this document records them. |
| **Created** | 2026-06-28 |

> **Why this matters.** (1) A real polity can adopt **Axiacracy** on entirely different
> infrastructure — MOS is just how we stress-test it cheaply. (2) Reviewers repeatedly attacked
> **MOS-specific** properties as if they were doctrine (e.g., "the simulation has ground truth that
> reality lacks"). That is a *MOS affordance*, **not** an Axiacracy claim. Keeping the two separate
> makes both the doctrine and the critique cleaner.

## 1. The rule of thumb
- **Axiacracy = the invariants.** What **any** value-flow-governed state must have — substrate-
  independent (true whether citizens are humans or agents, whether it runs on servers or a real
  bureaucracy, one region or a federation).
- **MOS = the free choices.** One realization's picks for *how* to instantiate the invariants for a
  cheap, observable, adversarially-testable simulation.
- **Examples are not doctrine.** The MOS examples woven through the methodology docs (the yogurt, the
  100-citizen P0, the Cognitive-Health ministry) are **illustrations**, not part of the invariant set.

## 2. The invariants — what any Axiacracy must have
1. **Multidimensional, perspectival value** — an Æ-vector as the *state frame's own lens* (federation
   of frames; no apex owner of value).
2. **Sensing vs. coercion separated**; **coercion graduated** by measurement-confidence × inter-frame
   scope; **soft power** where measurement is weak.
3. **Anti-value** as an independent, priced category; **restorative-first justice** (measure the
   harmful event → restore across axes → deter proportionally).
4. **Non-transferable civic standing (Æ)** distinct from a **thin money settlement rail** (money ≠
   civic power).
5. **Per-cohort, non-votable floors** (minority protection); **capability floors = availability of
   material means**, not audited functioning.
6. **Own-the-earned property**; **unearned rent (by observable signatures) → the commons**; a
   **democratically-chosen revenue mix**.
7. **Transparency-by-construction**, **contestability**, **non-retroactivity**, **versioned norms**.
8. **The Charter** (jus cogens) + norm hierarchy + eternity core + **constituent power**.
9. **Democratic weight-setting** + **adversarial, multi-source measurement** + **citizen-attestation
   accountability**; the **six citizen-influence channels**; organs scored by attested value; **roles
   held by human or AI on merit**.
10. **No governance signal movable by money**; the **measurement/accounting layer independently
    governed** (standards authority + sortition ratification).
11. **Bounded clawback** + **systemic-risk throttles**; **graduated, warranted, logged** intrusion.
12. **Unique identity** (anti-Sybil) + **graded personhood** + **naturalization throttle**; **universal
    inviolable rights**.

These hold for **any** Axiacracy. Change the substrate, and they still must hold.

## 3. The MOS choices — one realization (all replaceable)
| Dimension | MOS picks | A real Axiacracy could instead |
|---|---|---|
| **Who the citizens are** | 2,000–3,000 **AI agents** | humans, or a human/agent mix |
| **Runtime** | the **Orkestron stack** (orkestro.net / .dev / .ai, aeilus) | real civic infrastructure, other software |
| **Cost management** | **tiered cognitive fidelity (A/B/C)**, event-ticks, cohort reasoning | not needed with human citizens; different scaling |
| **Tamper-evidence** | a **Merkle** verifiable log | any tamper-evident public log; on-chain for federation |
| **Time** | a **sim-clock**; **ground truth available** (to score estimators) | real time; **no ground-truth oracle** (reality's honest limit) |
| **Scope** | **P0**: ~100 citizens, one region, a handful of ministries | full population, many regions, full ministry set |
| **Parameters** | specific numbers (`v_max`, escrow curves, thresholds, ladders) | each polity sets its own |
| **Purpose** | a **frontier-explorer** — map where governance stays stable vs. gets gamed | a live polity, not an experiment |

## 4. Consequences of the separation
- **The "sim has ground truth" objection dissolves.** Ground truth is a **MOS affordance** used to
  *test the estimators*; Axiacracy never claims a truth oracle in reality (Part III's adversarial
  measurement is precisely the answer to *not* having one).
- **The tiered-agents / Orkestron / Merkle critiques are MOS-level**, not doctrine-level — a real
  Axiacracy simply makes different implementation choices.
- **What the critique should target as *doctrine*** is only the §2 invariants (and their open items:
  the formal spec, the inter/intra-frame line, measurement-layer governance, confidence estimation,
  the missing pillars). Everything else is MOS.

## 5. Repository mapping
- **`methodology/`** = **Axiacracy** (the invariants + their rationale). *(MOS examples here are
  illustrative only.)*
- **`implementation/`** = **MOS** (the Orkestron mapping, tiers, sim-clock, P0 build).
- The **Full Specification** Parts 0–VII + IX are **doctrine**; **Part VIII (Implementation)** is the
  **MOS layer**; the compendium's §13 likewise.

## 6. The next structural step (proposed, not yet done)
Physically migrate the **MOS-specific** content (capacity strategy, Orkestron mapping, the P0 build,
numeric parameters) out of the doctrine docs into `implementation/`, leaving the methodology docs
**pure doctrine with illustrative examples clearly marked**. This makes Axiacracy independently
readable and adoptable, and MOS a clean, swappable realization beneath it.
