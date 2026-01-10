# The Context Primitive

**What Context Capture Requires**

---

## Why Context Is Non-Negotiable

The same question has different answers depending on who's asking, what they're doing, and what constraints apply.

- "Is this cost allowable?" depends on the award type, entity type, cost category, and timing.
- "Do I need prior approval?" depends on the threshold, the delegations in place, and the specific activity.
- "What's the right approach?" depends on risk tolerance, resources, and organizational culture.

Systems that ignore context produce generic answers. Generic answers are often wrong.

Context must be captured explicitly, not inferred or assumed.

---

## The Context Model

Context has multiple dimensions, each of which can affect outcomes:

### 1. Entity Context
Who or what is the actor?

**Attributes:**
- Entity type (individual, organization, government, nonprofit, etc.)
- Entity subtype (city, county, state agency, tribal, etc.)
- Size / scale (budget, employees, service population)
- Geographic scope (jurisdiction, service area)
- Registration status (SAM, state registrations, licenses)

**Why it matters:**
Different entity types have different rules. A state agency has different requirements than a nonprofit. A small organization may have different thresholds than a large one.

### 2. Role Context
What role is the actor playing?

**Attributes:**
- Role type (recipient, subrecipient, contractor, pass-through entity)
- Position (executive, manager, specialist, reviewer)
- Authority level (full decision authority, limited delegation, advisory only)
- Certification status (licensed, certified, designated)

**Why it matters:**
The same person in different roles has different authorities and obligations. A program manager approving a cost is different from an auditor reviewing it.

### 3. Lifecycle Context
What stage of work is this?

**Attributes:**
- Lifecycle stage (pre-award, award, implementation, closeout, audit)
- Phase within stage (planning, execution, reporting)
- Timing (year of award, reporting period, time remaining)
- Status (active, suspended, closed)

**Why it matters:**
Requirements change throughout the lifecycle. What's required at closeout differs from what's required at award. Deadlines create different constraints at different times.

### 4. Relationship Context
What relationships are relevant?

**Attributes:**
- Hierarchical relationships (awarding agency, pass-through, subrecipient)
- Peer relationships (partners, collaborators)
- Service relationships (contractors, vendors)
- Oversight relationships (auditors, monitors)

**Why it matters:**
Obligations flow through relationships. A recipient's duties to a funder differ from its duties to a subrecipient.

### 5. Domain Context
What subject matter applies?

**Attributes:**
- Domain (grants, procurement, finance, HR, etc.)
- Sub-domain (cost allowability, time and effort, procurement method)
- Activity type (direct service, administrative, capital)
- Risk category (high-risk, low-risk, standard)

**Why it matters:**
Different domains have different rules. A cost allowability question invokes different authority than a procurement question.

### 6. Governance Context
What governance applies?

**Attributes:**
- Regulatory framework (federal, state, local, international)
- Award terms (specific conditions, special conditions)
- Policy environment (internal policies, board directives)
- Delegation status (what's been delegated, what's retained)

**Why it matters:**
Governance determines which rules apply and how discretion is allocated.

---

## Context Resolution

When a question is asked, the system must resolve context:

1. **Identify the entity** — Who is asking, or who is the question about?
2. **Determine the role** — In what capacity is the actor operating?
3. **Establish lifecycle position** — What stage and phase?
4. **Map relationships** — What connections are relevant?
5. **Scope the domain** — What subject matter is involved?
6. **Apply governance** — What rules govern?

Each step narrows the applicable authority and shapes the answer.

---

## Context Capture Patterns

Context can be captured through:

### Explicit Declaration
The user or system explicitly states context.

*"I am asking as a grant manager for a city government about a federal award in Year 2."*

**Pros:** Clear and unambiguous
**Cons:** Burden on user; may be forgotten

### Profile-Based
Context is drawn from a pre-established profile.

*System knows: User is a grant manager at City of X, working on Award Y, currently in Year 2.*

**Pros:** Low friction; consistent
**Cons:** Requires setup; may become stale

### Session-Derived
Context accumulates during a session.

*User asked about Award Y earlier; system carries that forward.*

**Pros:** Natural flow; reduces repetition
**Cons:** Context can drift; may make incorrect assumptions

### Question-Inferred
Context is extracted from the question itself.

*Question mentions "FEMA grant" — system infers federal, disaster context.*

**Pros:** No extra input required
**Cons:** Inference can be wrong; requires confirmation

### Hybrid
Combination of patterns, with explicit overriding implicit.

*Profile provides baseline; session refines; user can override.*

**Pros:** Balances convenience and precision
**Cons:** Complexity; must handle conflicts

---

## Context-Dependent Authority

Context affects which authority applies:

| Context Dimension | Authority Affected |
|-------------------|-------------------|
| Entity type | Threshold requirements, reporting obligations |
| Role type | Approval authority, compliance requirements |
| Lifecycle stage | Active requirements, timing rules |
| Relationship | Flow-down requirements, monitoring duties |
| Domain | Substantive rules, standards |
| Governance | Applicable regulations, delegations |

Without context, authority is abstract. With context, authority is actionable.

---

## Context Gaps

When context is incomplete, the system must:

1. **Identify what's missing** — Which context dimensions are undefined?
2. **Assess impact** — Does the gap affect the answer?
3. **Request clarification** — Ask for the missing context
4. **Or refuse** — If the gap cannot be filled, refuse to answer

**Anti-pattern:** Assuming default context without disclosure.

If the system assumes "federal award" when the user hasn't specified, and the award is actually state-funded, the answer may be wrong. Assumptions must be visible and confirmable.

---

## Context as Scope Constraint

Context doesn't just inform answers. It constrains scope.

A system operating in a specific context should:
- Only offer options applicable to that context
- Only cite authority applicable to that context
- Only learn from examples in comparable contexts

This prevents:
- Irrelevant recommendations
- Misapplied precedent
- Scope creep

---

## Implementation Note

This document describes **what** context capture must support, not **how** to implement it.

Key implementation considerations:
- Context must be storable and retrievable
- Context changes must be trackable
- Context must be attachable to decisions
- Context must be comparable across instances

Specific schema design and interaction patterns depend on context and remain outside the scope of this research.

---

*Context is not metadata. It's the difference between right answers and relevant answers.*
