# The Authority Primitive

**How Authority Layers Compose**

---

## Why Authority Matters

In judgment-heavy domains, the question "What should I do?" is inseparable from "What am I required to do?"

Authority is the backbone of defensible decisions. Without explicit authority:
- Recommendations are opinions
- Decisions are preferences
- Conclusions are guesses

With explicit authority:
- Recommendations are traceable
- Decisions are grounded
- Conclusions are defensible

Decision intelligence requires authority to be **first-class**—not an afterthought, not a citation at the end, but the structural spine of reasoning.

---

## The Authority Hierarchy

Authority is not flat. It is layered, with higher layers governing lower layers.

### Layer 1: Constitutional / Statutory
The highest level of binding authority.

- Constitutions
- Statutes (USC, state codes)
- Treaties and international agreements

**Property:** Creates the legal foundation. Cannot be overridden by lower layers.

### Layer 2: Regulatory
Detailed implementation of statutory requirements.

- Federal regulations (CFR)
- State regulations
- Agency rules

**Property:** Implements statutory intent. Must be consistent with statutes.

### Layer 3: Guidance and Standards
Non-binding interpretation and professional norms.

- Agency guidance documents
- Professional standards (GAAP, GAGAS, etc.)
- Industry best practices
- FAQs and interpretive letters

**Property:** Clarifies application. Carries weight but not force of law.

### Layer 4: Contractual / Award Terms
Specific agreements governing particular relationships.

- Contracts
- Grant award terms
- Subaward agreements
- Service agreements

**Property:** Binds parties. Must be consistent with applicable law and regulation.

### Layer 5: Policy / Internal Governance
Entity-specific rules and procedures.

- Organizational policies
- Standard operating procedures
- Internal controls
- Delegation of authority

**Property:** Governs internal operation. Must be consistent with all higher layers.

### Layer 6: Operational Decisions
Specific choices within the governed framework.

- Individual decisions
- Approvals
- Interpretive choices

**Property:** Occurs within constraints of all higher layers.

---

## Authority Resolution

When a question arises, authority must be resolved from top to bottom:

1. **Is there statutory authority?** If yes, it governs.
2. **Is there regulatory implementation?** If yes, it specifies.
3. **Is there guidance?** If yes, it clarifies.
4. **Are there award terms?** If yes, they apply (within legal limits).
5. **Is there internal policy?** If yes, it governs (within all higher limits).
6. **Is there precedent?** If yes, it informs.

At each layer, the question is: **Does this layer say something, and is it consistent with higher layers?**

---

## Conflict Resolution

Conflicts between authority layers are resolved by **precedence**:

- Higher layers override lower layers
- More specific provisions override general provisions (at the same level)
- Later provisions override earlier provisions (at the same level)
- Explicit terms override implied terms

When conflicts cannot be resolved by rule, they become **interpretive questions** requiring human judgment and potentially formal clarification.

---

## Authority Types

Not all authority is the same type. The type affects how it's used:

### Mandatory
Must be followed. No discretion.

*"The recipient shall..."*
*"...is required to..."*
*"...must..."*

### Prohibitive
Must not be done. No discretion.

*"The recipient shall not..."*
*"...is prohibited..."*
*"...may not..."*

### Permissive
Allowed but not required. Discretion exists.

*"The recipient may..."*
*"...is allowed to..."*
*"...at the discretion of..."*

### Conditional
Applies only when conditions are met.

*"If... then..."*
*"When... the recipient shall..."*
*"Unless... the requirement applies..."*

### Delegative
Creates authority for someone else to decide.

*"The pass-through entity shall determine..."*
*"...as approved by..."*
*"...subject to agency discretion..."*

---

## Authority Attributes

Each authority should have:

### Citation
Precise location in source hierarchy.

- Title, section, subsection
- Effective date / version
- Amendment history

### Scope
What does this authority govern?

- Subject matter
- Entity types
- Geographic boundaries
- Time periods

### Applicability Conditions
When does this authority apply?

- Triggering conditions
- Exclusions
- Thresholds

### Relationships
How does this authority connect to others?

- Implements (points to higher authority)
- Implemented by (points to lower authority)
- Cross-references (parallel authority)
- Supersedes (replaces prior authority)

---

## The Authority Chain

For any decision, the system should be able to produce an **authority chain**:

```
Decision: "Is this cost allowable?"

Authority Chain:
├── Statute: 31 USC 6301 (Federal Grant and Cooperative Agreement Act)
├── Regulation: 2 CFR 200.403 (Factors affecting allowability)
├── Guidance: Compliance Supplement Part 3 (Cost Principles)
├── Award Terms: Special Condition 14 (Prior approval requirements)
└── Entity Policy: Procurement Policy Section 4.2 (Approval thresholds)
```

This chain is:
- **Traceable** — Each link points to a source
- **Defensible** — Each link has legal or contractual basis
- **Complete** — All governing layers are represented
- **Consistent** — No unresolved conflicts

---

## First-Class Refusal from Authority Gaps

When authority cannot be established, the correct behavior is **refusal**, not guessing.

**Refusal triggers:**
- No governing authority found
- Conflicting authority unresolved
- Authority requires interpretation beyond system capability
- Applicability conditions unclear

**Refusal output:**
- Statement of what's missing
- Specification of what would be needed
- Guidance on who could provide it

This is not a failure. It's correct behavior. A system that always produces answers is a system that sometimes lies.

---

## Implementation Note

This document describes **what** authority structure must support, not **how** to implement it.

Key implementation considerations:
- Authority sources must be versioned (law changes)
- Citations must be parseable (for linking)
- Hierarchies must be traversable (for chain construction)
- Conflicts must be flagged (for human resolution)

Specific schema design and storage patterns depend on context and remain outside the scope of this research.

---

*Authority is not bureaucracy. It's the difference between opinion and position.*
