# Citizenship, Membership & Personhood — who is a member, and can a citizen be an AI?

| | |
|---|---|
| **Status** | **DRAFT v0.1 — under discussion** |
| **Fills** | gap **G4** (citizenship + AI-agent personhood + anti-Sybil identity) — and, because unique identity is the bedrock, closes the Sybil attack surface under voting/attestation/delegation/recognition. |
| **Created** | 2026-06-28 |

> A polity must say **who its members are**, how one **joins and leaves**, and — uniquely here —
> **whether a citizen may be an AI agent** (a live question the MOS simulation exists to explore).
> Underneath all of it sits the one foundation the whole governance layer depends on: **unique,
> verifiable identity.**

## 1. Identity is the bedrock (anti-Sybil)
Every governance mechanism — voting weights, value-attestation, delegation, peer recognition —
**collapses if identities can be multiplied.** So **every member has a unique, verifiable civic
identity:**
- **Humans:** a DID + **proof-of-personhood** (biometric-uniqueness / social-graph / attestation-based
  — a hard, actively-researched problem, flagged as such).
- **Agents:** a **registered, non-cloneable, auditable agent instance** with a **responsible entity**
  behind it — **no anonymous mass-minting.**
**One identity = one vote-weight and one attestation-weight**, regardless of type. Without this layer,
nothing above it is safe.

## 2. Membership is a value-participation relationship
A member is a value transformer **recognized as part of the polity's value system**, holding civic
**rights** (vote, floors, recognition, standing) and **duties** (conformance to the Charter,
contribution). Entry routes:
- **Birth / origination** (humans born in the polity; the polity's rule for originated agents, if any).
- **Naturalization** — a **process**, not a mint: demonstrated participation + conformance over time,
  ratified. (This is the throttle that stops instant mass-citizenship.)
- **The polity constitutionally decides whether — and which — AI agents may be members** (§3).

## 3. AI-agent personhood — a graded status, not a binary
Rather than "AI is/ isn't a citizen," standing is granted in **tiers**, each with matching rights **and**
accountability:

| Tier | What it is | Rights | Accountability |
|---|---|---|---|
| **Tool** | a service | none of its own | its **principal** is fully responsible |
| **Delegate** | an agent acting *for* a human/entity (a proxy, a party-agent) | **delegated** standing, bounded by its principal | the **principal** is accountable |
| **Autonomous participant** | recognized to hold roles, contribute, accrue standing in its own right | role-holding + standing | a **human/entity liability backstop** (D4) |
| **Full civic person** | vote, own produced goods, sue, be liable | full civic rights | its own liability + the anti-Sybil + naturalization gates |

**"A citizen may be an AI if the polity so decides"** = a constitutional grant of the **Full-civic-person**
tier, gated by unique-identity + naturalization. (Æ/standing is non-transferable regardless, so even a
full-person agent cannot buy or inherit civic power.)

## 4. The AI-vote-swarm defense
If agents can vote, the polity **must** control minting or a sponsor spins up a million voters:
- **Unique costly identity** (no free cloning) + **a cap/rate on agent-citizen creation**;
- **agent citizenship is *naturalized*, not minted** — earned via demonstrated value contribution over
  time, never instant;
- optionally, **weight/caps on agent votes relative to humans**, a per-polity choice.
So agent enfranchisement is **slow, identity-gated, and contribution-earned** — the swarm attack needs
mass unique naturalized identities, which the gates deny.

## 5. Exit — and you cannot exit to escape liability
**Exit** is an inviolable right (Charter). But exit is **renunciation of membership + its rights/duties**,
and **outstanding liabilities settle first** — you cannot exit the *ledger* to dodge an anti-value
debt (this closes the capital-flight loophole, C2). You cannot selectively exit *measurement/monitoring*
while keeping residency and floors: membership is a package.

## 6. Non-members
Foreign persons/agents and visitors interact **at the boundary** (external flows), with **no vote and
no floors** — **but the inviolable rights (life, bodily integrity, consent) are universal**, held by
*anyone in the jurisdiction*, not just members (this is a rights floor, not a membership privilege).
Ties to the External-Relations ministry and foreign-frame recognition.

## 7. Where MOS sits (a boundary note)
**MOS is the extreme case:** a polity populated **entirely by AI-agent citizens** — i.e., MOS grants
(simulated) agents the full-person tier, which makes it the ideal **test bed** for exactly the
agent-citizenship dynamics (swarm defense, naturalization, identity). **Axiacracy the doctrine is
agnostic:** a real instance may be all-human, mixed, or agent-inclusive. MOS picks one setting to
stress-test; the doctrine only fixes the *invariants* above (unique identity, graded personhood,
naturalization throttle, non-transferable standing, universal inviolable rights).

## Open items
- The proof-of-personhood mechanism (the hardest sub-problem) and its failure modes.
- Naturalization criteria + the agent-citizen creation cap/rate.
- Whether agent votes are weighted vs human votes (per-polity, but needs a default).
- Originated-agent origin rules (who may create an agent that could later naturalize).
