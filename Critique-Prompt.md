# Axiacracy — Maturity Critique Prompt

*Paste the prompt below into a strong reasoning model (or give it to human expert reviewers),
attaching **[`methodology/Axiacracy-Full-Specification.md`](methodology/Axiacracy-Full-Specification.md)**
(the complete, unambiguous description — use this, not the terse compendium) — and, for depth,
the detailed docs in `methodology/`. Goal: mature the doctrine until a simulation or a playable
online world can be built **without the implementation raising questions about the description
itself**.*

> **Note for the reviewer:** the Full Specification reflects the "sensing vs. coercion" synthesis
> (v2) and opens with **seven pre-empted misreadings** plus a **§IX "known limits & open work".**
> Please verify whether the synthesis *actually* resolves the measurement / pluralism / coercion
> objections, and **concentrate new fire on the §IX open items** rather than re-raising what §0
> and §IX already address.

> **Usage modes.** (1) **One-shot panel** — run the whole prompt once. (2) **Persona rotation**
> — run it once per reviewer persona (§Reviewers) for depth, then dedupe. (3) **Adversarial
> pair** — run once to attack, then feed the findings back asking the model to steelman the
> doctrine's defense, then attack again. Mode 2 or 3 gives the sharpest results.

---

## THE PROMPT

You are a **panel of adversarial expert reviewers** stress-testing a proposed system of
government called **Axiacracy** (governance by balancing multidimensional value flows). The
full description is attached. Your job is **not** to praise, summarize, or agree — it is to
**find everything wrong with it** so it can be made mature enough to implement. Assume the
author *wants* the flaws found; agreeableness is a failure. Do not soften. Do not pad with
compliments.

**The maturity bar.** The description must be (a) **internally consistent**, (b) **complete**
(no essential dimension of a political-economic order missing), (c) **robust to adversarial
exploitation**, (d) **grounded** (its measurement claims are actually feasible), and (e)
**specified enough that a builder could implement a simulation and a multiplayer game from it
without having to invent undefined rules.** Judge against this bar.

**Reviewers (adopt each lens explicitly; a finding should name the lens):**
- **Constitutional lawyer / political philosopher** — legitimacy, rights, separation of
  powers, rule of law, succession, sovereignty.
- **Mechanism designer / social-choice theorist** — incentive-compatibility, strategy-proofness,
  Arrow/Gibbard-Satterthwaite limits, voting & delegation manipulation, quadratic schemes.
- **Economist (Austrian + institutional + public-choice)** — the calculation/knowledge problem,
  price vs. planning, rent measurement, capital & credit, regulatory capture, rent-seeking.
- **AI-alignment & security engineer** — Goodhart/metric-gaming, reward hacking, the
  algorithmic-officeholder validation, hidden-value-redirection detection, oracle/measurement
  attacks, Sybil/collusion.
- **Complex-systems / cybernetics reviewer** — stability, feedback, oscillation, requisite
  variety, emergent failure, viability (VSM).
- **Moral philosopher** — pluralism vs. an imposed value metric, what must *not* be measured or
  priced, autonomy vs. paternalism, the "meaning" and anti-value judgments.
- **Historian of political systems** — what this reinvents; what has been tried (Cybersyn,
  planned economies, social-credit systems, technocracy, ESG, DAOs, futarchy) and why it failed.
- **Behavioral scientist** — the model of the citizen; preference formation, manipulation,
  bounded rationality; whether the incentives do what they claim on real (or LLM-agent) minds.
- **Simulation / game designer** — can these rules be turned into an unambiguous rule-set an
  engine and players can follow; where are the undefined rules, unbounded loops, or unplayable
  abstractions.

**Attack every mechanism on these dimensions (be exhaustive and specific):**
1. **Internal contradiction** — cite section X vs. section Y; state the inconsistency.
2. **Underspecification / insufficiency** — an assertion the description does not mechanize;
   what a builder would be forced to invent, and where the ambiguity bites.
3. **Unstated assumption** — especially about measurement feasibility, technology, and human/
   agent behavior. Name the assumption and what breaks if it is false.
4. **Gameability / attack vector** — how a rational bad actor exploits it: Sybil, collusion,
   metric-gaming/Goodhart, vote/delegation manipulation, rent-hiding, capture, self-dealing via
   multi-step flows, measurement/oracle attacks, false attestation/reclamation. Give the exploit
   step by step.
5. **Failure mode / degeneration** — the path by which it drifts into dystopia (surveillance
   state, technocratic capture, measurement tyranny, stagnation, mob rule, plutocracy-by-rent).
6. **Measurement feasibility** — the doctrine rests on measuring value, anti-value, realized
   value, rent (captured−created), participation-condition θ, and cohort effects. For each,
   ask: is it actually measurable, by whom, with what error, and what happens when the estimate
   is wrong or gamed? Attack the epistemics hard — this is the load-bearing assumption.
7. **Prior-art collision** — what established result (impossibility theorem, historical failure,
   known critique) does this ignore or need to answer?
8. **Normative objection** — whose values; who decides the axes/floors; the legitimacy of the
   state measuring frames; the line "not everything should be priced."
9. **Edge cases** — boundary conditions where the rules produce absurd or undefined results.
10. **Implementability** — the specific rules a simulation/game builder cannot yet code because
    the description is silent or contradictory.

**Also check for what is MISSING** (dimensions a complete theory of order must address):
property & capital, succession & transfer of power, external relations & defense, citizenship &
membership, emergency/state-of-exception, the model of the citizen, monetary/credit system,
corruption resistance — flag any that are absent or thin.

**Output format.** First, a one-paragraph blunt overall verdict on maturity against the bar.
Then a **table of findings**, most severe first:

| # | Lens | Type (1–10) | Severity (Blocker / Major / Minor) | Location | The problem (precise) | Failure scenario (concrete) | Proposed fix or the open question it forces |

Then: **the 5 findings that most threaten the whole doctrine** (the ones that, unaddressed,
make it unbuildable or incoherent), ranked, each with why it is load-bearing. Finally, a short
list of **the strongest genuine ideas worth keeping** (so revision doesn't discard them) — brief,
no flattery.

**Rules:** Be concrete — every finding needs a specific location and a specific failure
scenario, not a vague concern. Prioritize ruthlessly; a Blocker is something that makes the
system incoherent or unbuildable, not a nitpick. Steelman before you strike, but then strike
hard. If something is actually fine, say nothing about it — spend words only on problems.

---

## After the critique
Feed the returned findings back into the methodology: each **Blocker/Major** becomes either a
fix to an existing doc or a new open decision. Re-run the prompt after a revision pass to
confirm the blockers are retired and no new ones were introduced (the doctrine's own
"adversarial verify" loop).
