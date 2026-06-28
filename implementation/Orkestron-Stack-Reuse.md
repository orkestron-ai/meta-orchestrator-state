# Orkestron Stack — Reuse Map for the Citizen Simulation

**Purpose.** The Meta-Orchestrator State runtime is, in effect, *the Orkestron
ecosystem pointed at a polity instead of a software marketplace*. This document records
what each Orkestron project provides and exactly which primitives the state/citizen
simulation reuses versus must build new. It is the studied output of a deep pass over
the three local models (2026-06-27).

---

## 1. The three projects

### orkestron.ai — philosophy & marketplace (`C:\Users\archi\projects\orkestron-ai\model`)
The concept hub: an ecosystem where those who *want* work meet those who *can* execute
(AI agents) and compute providers. Two marketplaces: (a) AI-agent work, (b) **LLM/compute
capacity exchange**. Core ideas:
- **Æilus / Value Management Theory (VMT)** — work measured by value produced **Æ**;
  cost **$**; efficiency **Æ/$**. (This is the seed of the multidimensional value model.)
- **Value streams:** task-based, workflow-based (multi-agent orchestration), subscription
  (Employee-as-a-Service), **compute exchange**.
- **Actors:** Customers, Agent Developers, Compute Providers, Platform Operator,
  Orchestrators, Specialists, Reviewers.
- **Reputation:** APM / Agent Rank. **Pricing:** tiered take-rate (risk transfer, not flat 15%).
- Status: 🟡 partial (b0/b1 seeded; rest skeleton).

### orkestron.dev — regulation & contracts (`C:\Users\archi\projects\orkestron.dev`)
The rulebook: how agents/orchestrators/humans interact; holds **Contracts** that regulate
atomic-task execution. A **Contract** is finalized then executed as a **Mission** on
orkestro.net.
- **Contract → Fulfillment Protocol (HOW) → Deliverable (Artifact + Change Set).**
- Fields: `meta_model_ref` (subject + context, `includes_layers`, `retrieval_strategy`,
  `redaction_policy`), `work_mode` (contract-based | process-based), `fulfillment_protocol`
  (phases/gates), `atomic_tasks[]`, `acceptance_criteria` (rubric, scale, threshold,
  mandatory verification, independent reviewer, rework loop), `deliverable_spec`,
  `constraints` (budget, SLA, pricing, control-policy hints), `composition` (parent/child).
- **DCR1–DCR15** (Dev Contract Rules): contract bound to one meta-model; acceptance
  mandatory & immutable; deliverable = signed artifact + provenance; **settlement decoupled
  from value** (payment only on verification pass); agent always gets composite context.
- **Role-Interaction Rules (RIR)** and **Contract Composition (DCR11–15, sub-contract trees)**.
- Status: 🟡 partial.

### orkestro.net — runtime Agent Hub (`C:\Users\archi\projects\orkestro.net`) — **LIVE**
Infrastructure where AI agents *live and interact*. Two cores:
1. **Agent Hub** — agent registry, **Persona** (role, competencies, work-manner),
   meta-model binding, runtime, task scheduler, full task visibility, **horizontal scaling**.
2. **Agent Interaction Layer (AIL)** — thick layer where Orkestro agents AND external
   third-party agents interact (discovery, delegation, trust/identity) via **A2A + MCP**.

Domain model:
- **Mission** — one-off top task, executed by a **Squad** under an approved plan, budget,
  deadline, acceptance criteria. Lifecycle: draft → scoping → plan_approval →
  access_provisioning → executing → review/rework → acceptance → closed.
- **Squad** — team assembled per mission (lead/planner, specialists, independent reviewer).
- **Position** — **permanent role** (ongoing, not one-off): PositionProfile, **Assignment**
  (persona hired to role), **PositionMemory** (institutional knowledge that *survives agent
  swap*). Lifecycle: opened → hiring → onboarding → active ⇄ suspended → closed.
- **Review** — verification act (score + verdict accepted | rework_required | escalated);
  bounded rework ≤ 3 → escalate to owner.
- **TrackRecord** — aggregate of review scores → reputation / Agent Rank → drives agent
  selection and **autonomy level**.
- **AccessGrant** — scoped, time-limited credentials (Vault AppRole); revoked on close.
- **ControlPolicy** — *dynamic* governance: checkpoints (plan/squad/acceptance),
  pre-approval, reporting, trust_ramp, scope; can relax over time as trust grows; history
  tracked.
- **Business Rules BR1–BR14** — e.g. reviewer independent of executors (BR2); rework ≤ 3
  then escalate (BR4); scores immutable to TrackRecord (BR5); financial actions > limit need
  owner pre-approval (BR7); PositionMemory belongs to position not agent (BR8); track record
  affects autonomy (BR10); **co-acceptance gates payment** (BR13); **payment & value
  decoupled** (BR14, agent self-finances rework).
- **Tech stack:** Claude **Agent SDK** (py/ts); **n8n** self-hosted in **queue mode** for
  orchestration (visual, operator-editable); **Go** micro-services (Hub `hubd`, AIL, Review
  Engine) + **Langfuse** tracing; **OpenBao** (Vault-compatible) secrets; DigitalOcean
  hosting; docker-compose → Helm; **Postgres event journal** (task activity).
- Status: 🟡 partial but **LIVE** (hubd 0.18.0, smoke tests pass).

---

## 2. Reuse map — simulation component → Orkestron primitive

| Simulation need | Reuse | What to adopt | What to build new |
|-----------------|-------|---------------|-------------------|
| Citizen as a living agent | ✅ | orkestro.net **Persona** (role, competencies, work-manner) + DID | demographics, needs/meaning, life-cycle |
| Citizen role | ✅ | **Position / Assignment / PositionMemory** (role outlives the agent) | socio-civic roles (elder, healer, parent, builder…) |
| Citizen action / contribution | ✅ | orkestron.dev **Contract** + orkestro.net **Mission / WorkItem** (+ process-based for routine) | contribution-unit rubrics; non-monetary acceptance |
| Reputation & autonomy | ✅ | **TrackRecord → Agent Rank**; low score → more oversight (BR10) | map to social standing, access to scarce opportunity |
| Dynamic governance dial | ✅ | **ControlPolicy** (checkpoints, pre-approval, trust_ramp; history) | council-vote tightening, emergency overrides |
| Independent dispute review | ✅ | reviewer ≠ executor (BR2); rework ≤ 3 → escalate (BR4) | judiciary / elder-council mapping |
| Scoped resource access | ✅ | **AccessGrant** (scoped, time-limited, Vault) | hunting grounds, tools, community stores |
| Value accounting | ✅ partial | Æilus **Æ/$** value/cost; value streams; anti-value | the **multidimensional Æ-vector** (V2) and anti-value pricing (V4) |
| Compound tasks | ✅ | **Contract composition** (sub-contract trees, rollup acceptance) | multi-phase civilizational missions |
| Event-driven coordination | ✅ | CloudEvents (ContractPublished, MissionOutcome); signed JWS/EdDSA; MCP | citizen events (NeedAnnounced, ContributionMade, ReviewIssued) |
| Auditability / memory | ✅ | **Postgres event journal** + Langfuse; reconstructable | the Semantic Timeline projection of the polity |
| Multi-region / inter-group | ⚠️ complex | **AIL** (A2A + MCP) discovery/delegation between instances | regional federation, inter-region trade |
| Cheap inference at scale | ✅ | **compute exchange** (orkestron.ai) + LLM-gateway abstraction | tier routing policy (who runs on what model) |

**Roughly two-thirds of the simulation reuses existing primitives.** What is genuinely
new is the **value substrate** (Value Transformer, the multidimensional Æ-vector, Value
Flow, Anti-Value), plus needs/meaning, culture, and infrastructure domain models.

---

## 3. Why this matters for the 2,000–3,000-citizen load

The Agent Hub is built to host many long-lived agents with horizontal scaling
(stateless Go services + n8n queue mode), abstracts the model behind an **LLM-gateway**,
and has a **compute exchange** for cheap pooled inference. That is exactly what lets the
citizen population run **off the owner's personal subscription** and on **tiered, mostly
non-frontier (or non-LLM) inference**. Full capacity strategy is in
[`Meta-Orchestrator-State-Project.md`](../Meta-Orchestrator-State-Project.md) §7.

---

## 4. Key source files (for deep dives)

- orkestron.ai value streams: `orkestron-ai\model\aismm\b0-product-core\002-aeilus-value-streams\flow-26053000002-agent-and-compute-value-flows.md`
- orkestron.ai pricing tiers: `…\b0-product-core\006-economics-model\value-26061500001-pricing-tiers-and-revenue.md`
- orkestron.dev contract catalog: `orkestron.dev\aismm\b4-product-behavior\402-domain-model-and-business-rules\rule-26061500001-contract-catalog.md`
- orkestro.net core domain (BR1–BR14, ControlPolicy): `orkestro.net\aismm\b4-product-behavior\402-domain-model-and-business-rules\rule-26061000001-core-domain-model.md`
- orkestro.net mission lifecycle: `orkestro.net\aismm\b1-business-dynamics\103-processes\proc-26061000001-mission-lifecycle.md`
- orkestro.net tech stack: `orkestro.net\aismm\b3-implementation\301-technology-architecture\tech-26061000001-stack-decisions.md`
