# The Decision Primitive

**What a Decision Record Must Contain**

---

## Why Decisions Are the Unit of Value

Workflows track what happened.
Analytics track what the data shows.
Decisions track **what was chosen, by whom, with what reasoning, under what authority**.

In judgment-heavy domains, the decision is the atomic unit of value—not the task, not the report, not the output.

Capturing decisions structurally is the foundation of decision intelligence.

---

## The Minimum Viable Decision Record

A decision record that supports governance, learning, and accountability must contain:

### 1. Identity
Every decision needs a stable identifier that persists across time and context.

- **Decision ID** — Unique, immutable reference
- **Decision type** — Classification (e.g., allowability, eligibility, approval, allocation)
- **Version** — If decisions can be revised, the version chain must be traceable

### 2. Context
The same question has different answers depending on context. Context must be captured explicitly.

- **Entity** — Who or what is the decision about?
- **Role** — What role is the decision-maker acting in?
- **Stage** — What phase of the lifecycle is this decision occurring in?
- **Scope** — What boundaries constrain the decision?
- **Timestamp** — When was the decision made?

### 3. Question
What exactly was being decided?

- **Question statement** — The decision prompt in clear language
- **Question type** — Binary, choice, allocation, prioritization, etc.
- **Options considered** — What alternatives were evaluated?

### 4. Inputs
What information was available at decision time?

- **Evidence consumed** — Documents, data, prior decisions
- **Context state** — Relevant conditions at decision time
- **Missing inputs** — What was unknown or unavailable?

### 5. Authority
What rules, requirements, or standards governed this decision?

- **Primary authority** — The governing rule or requirement
- **Authority chain** — How authority was traced (statute → regulation → policy → terms)
- **Interpretive basis** — If authority required interpretation, what was the basis?
- **Precedent** — Any prior decisions that informed this one

### 6. Reasoning
How did the decision-maker arrive at the conclusion?

- **Logic chain** — The sequence of inference
- **Factors weighed** — What considerations mattered?
- **Trade-offs made** — What was sacrificed for what?
- **Confidence level** — How certain is the conclusion?

### 7. Outcome
What was decided?

- **Decision outcome** — The actual choice made
- **Conditions** — Any contingencies or qualifications
- **Effective date** — When the decision takes effect
- **Expiration** — If applicable, when the decision expires

### 8. Accountability
Who is responsible?

- **Decision maker** — The human who made or ratified the decision
- **Delegation chain** — If delegated, from whom?
- **Review status** — Has the decision been reviewed?
- **Override history** — Any changes or reversals

### 9. Downstream
What happens next?

- **Required actions** — Tasks or follow-ups triggered
- **Dependent decisions** — Other decisions that depend on this one
- **Monitoring requirements** — Ongoing obligations created

---

## Properties of Well-Formed Decision Records

### Immutable Core
Once recorded, the core decision record should not change. Revisions create new versions with explicit links to prior versions.

### Complete Provenance
Every field should be traceable to its source. "Where did this come from?" should always have an answer.

### Traversable Authority
The authority chain should be navigable. From any decision, you should be able to walk up to the governing statute and down to the specific application.

### Explicit Uncertainty
If something is unknown, it should say so. Missing inputs, low confidence, and interpretive gaps should be visible, not hidden.

### Learning-Ready
The structure should support pattern extraction. Decisions with similar contexts and authorities should be findable and comparable.

---

## What Decision Records Enable

### For Individuals
- Reduced cognitive load (the system remembers)
- Defensible positions (the reasoning is preserved)
- Faster decisions (precedent is available)

### For Organizations
- Institutional memory (decisions survive turnover)
- Consistent application (similar cases treated similarly)
- Audit readiness (evidence is pre-organized)

### For Systems
- Pattern learning (what works, what doesn't)
- Gap detection (what's missing from authority)
- Drift monitoring (are decisions consistent over time?)

---

## The Anti-Pattern: Decisions Without Structure

Most organizations make decisions constantly. Almost none capture them structurally.

Instead, decisions exist as:
- Emails ("Per our discussion, we're going with Option B")
- Meeting notes ("Team decided to proceed")
- Memory ("We've always done it this way")
- Artifacts ("The approved budget shows...")

This creates:
- Loss when people leave
- Inconsistency across cases
- Audit scrambles
- Learning that doesn't compound

The decision primitive fixes this—not by adding overhead, but by making structure a byproduct of operation.

---

## Implementation Note

This document describes **what** a decision record must contain, not **how** to implement it.

Implementation details—schema design, storage architecture, API patterns—depend on context and remain outside the scope of this research.

The primitive is the requirement. The implementation is the solution.

---

*Decisions are the unit of judgment. Structure is how they compound.*
