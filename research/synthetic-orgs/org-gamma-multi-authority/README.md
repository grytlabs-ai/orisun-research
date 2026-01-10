# Synthetic Organization: Gamma-MultiAuthority

**Archetype: Multi-Authority Environment**

---

## Purpose

This synthetic organization exhibits properties of a **multi-authority environment**:
- Decisions cross organizational roles
- Authority is layered and sometimes contested
- Escalation paths exist but are not always clear
- Multiple valid interpretations may coexist

It reveals requirements for **authority resolution, conflict handling, and governance mechanisms**.

---

## Entity Profile

| Attribute | Value |
|-----------|-------|
| Entity ID | gamma-001 |
| Entity Type | Federated Organization |
| Subtype | Multi-stakeholder partnership |
| Size Class | Medium-Large (variable by function) |
| Geographic Scope | Multi-jurisdictional |
| Primary Domain | Coordinated service delivery |

---

## Multi-Authority Characteristics

### Overlapping Jurisdictions
Multiple authorities govern the same activities.

| Activity | Authority A | Authority B | Authority C |
|----------|-------------|-------------|-------------|
| Hiring | Federal labor law | State employment law | Internal HR policy |
| Procurement | Federal acquisition regs | Funder-specific terms | Entity procurement policy |
| Data handling | Federal privacy law | State data protection | Contractual requirements |
| Reporting | Statutory requirements | Funder requirements | Board requirements |

**Consequence:** No single authority resolves most questions. Resolution requires traversing multiple sources.

### Contested Authority
Some decisions have legitimately competing authorities.

| Scenario | Stakeholder A Position | Stakeholder B Position |
|----------|------------------------|------------------------|
| Resource allocation | "Federal priority governs" | "Local need should determine" |
| Risk tolerance | "Conservative interpretation required" | "Flexible interpretation permitted" |
| Timeline | "Regulatory deadline is fixed" | "Extension precedent exists" |

**Consequence:** Resolution requires explicit governance mechanisms, not just rule lookup.

### Delegated Authority Chains
Authority flows through multiple levels with potential gaps or conflicts.

```
Original Authority (Statute)
    └── Implementing Authority (Regulation)
        └── Awarding Authority (Agency)
            └── Pass-Through Authority (Recipient)
                └── Operating Authority (Subrecipient)
                    └── Executing Authority (Staff)
```

At each level:
- Authority may be narrowed
- Conditions may be added
- Interpretation may vary
- Documentation may be incomplete

**Consequence:** "Who actually has authority here?" is a non-trivial question.

---

## Role Structure (Complex)

| Role | Nominal Authority | Actual Authority | Tension |
|------|-------------------|------------------|---------|
| Executive Director | Strategic decisions | Constrained by board, funders, regulations | May believe they have more authority than they do |
| Program Director | Program decisions | Subject to federal, state, funder requirements | Often caught between stakeholder demands |
| Compliance Officer | Advisory on compliance | No line authority; influence only | Must persuade, cannot direct |
| External Funder Rep | Award-specific requirements | Limited to award scope | May overreach into operational decisions |
| Board Member | Governance oversight | Fiduciary, not operational | May blur governance/management line |

---

## Decision Scenarios Under Multi-Authority

### Scenario M1: Conflicting Requirements
```
Situation:
- Federal regulation requires X
- Funder-specific terms require Y
- X and Y are in tension (not direct conflict, but difficult to satisfy both)

Question: How do we proceed?

Authority Analysis:
- Federal regulation has force of law
- Funder terms are contractual
- Contractual terms cannot override law
- But both must be satisfied if possible

Resolution Path:
1. Determine if true conflict or apparent conflict
2. If apparent: find interpretation satisfying both
3. If true: federal law governs; document; notify funder
4. If unclear: escalate for formal interpretation

Required Infrastructure:
- Conflict detection
- Precedence rules
- Escalation routing
- Resolution documentation
```

### Scenario M2: Authority Gap
```
Situation:
- Decision required for novel circumstance
- No clear authority addresses this exactly
- Multiple parties claim interpretive authority

Question: Who decides?

Analysis:
- Check delegation chains for gaps
- Identify who has been delegated similar authority
- Determine if formal interpretation needed
- Assess risk of proceeding without clarity

Resolution Path:
1. Document the gap explicitly
2. Identify parties with colorable authority claims
3. Convene for resolution or escalate
4. If time-critical: proceed with documentation; accept risk
5. Capture outcome as precedent for future

Required Infrastructure:
- Gap detection
- Stakeholder mapping
- Convening/escalation mechanism
- Precedent capture
```

### Scenario M3: Competing Interpretations
```
Situation:
- Regulation is ambiguous
- Funder interprets one way
- Legal counsel interprets another way
- Program staff have operational concerns with both

Question: Which interpretation governs?

Analysis:
- Neither interpretation may be "wrong"
- Risk profiles differ
- Operational implications differ
- Relationship implications differ

Resolution Path:
1. Document all interpretations with rationale
2. Assess risk profile of each
3. Identify who bears the risk
4. Decide based on risk tolerance + authority
5. Document decision rationale explicitly

Required Infrastructure:
- Interpretation capture (multiple positions)
- Risk assessment framework
- Authority-to-risk mapping
- Decision documentation with rationale
```

---

## Governance Mechanisms Required

### Escalation Paths
Not just "who to ask" but structured routing:

| Trigger | Escalation Target | Expected Output |
|---------|-------------------|-----------------|
| Conflict detected | Compliance + Legal | Interpretation memo |
| Authority gap | Executive + Counsel | Authority designation |
| Competing interpretations | Governance committee | Binding interpretation |
| External authority question | Funder/Agency | Formal written guidance |

### Resolution Documentation
Every resolution must capture:
- What was the question?
- What authorities were considered?
- What was the conflict/gap/ambiguity?
- Who participated in resolution?
- What was decided?
- What is the precedential value?
- When does this expire or require re-evaluation?

### Override Mechanisms
Sometimes authorized personnel must deviate from standard interpretation:
- Override authority must be explicit
- Override rationale must be documented
- Override must be flagged for review
- Pattern of overrides may indicate need for policy change

---

## Observations (Structural)

### What Alpha and Beta Infrastructure Misses

| Simpler Archetypes Assume | Gamma Reality |
|---------------------------|---------------|
| Single authority source | Multiple competing sources |
| Clear precedence | Contested precedence |
| Role = Authority | Role ≠ Authority (it's complicated) |
| Resolution is lookup | Resolution requires judgment + process |

### Additional Infrastructure Requirements

| Requirement | Rationale |
|-------------|-----------|
| Multi-source authority storage | Must represent overlapping/competing authorities |
| Conflict detection | Identify when authorities are in tension |
| Stakeholder registry | Know who has voice in resolution |
| Escalation workflow | Route unresolved questions appropriately |
| Interpretation capture | Store reasoned positions, not just outcomes |
| Precedent system | Prior resolutions inform future ones |
| Override tracking | Deviations visible and reviewable |

### The Human Judgment Layer

Multi-authority environments cannot be fully automated. They require:
- Judgment about which conflicts are real vs. apparent
- Judgment about risk tolerance
- Judgment about stakeholder management
- Judgment about when precedent applies

Infrastructure supports this judgment. It does not replace it.

---

## Findings

### F1: Authority Is Graph, Not Hierarchy
In multi-authority environments, authority relationships form a graph with cycles, not a clean tree. Infrastructure must handle this complexity.

### F2: Conflict Is Normal
Conflicts are not failures—they're the natural state of complex governance. Infrastructure must normalize conflict detection and resolution.

### F3: Interpretation Is First-Class
The "right answer" often doesn't exist until someone interprets. Interpretation must be captured, reasoned, and precedent-forming.

### F4: Governance Requires Process
Rules alone cannot resolve multi-authority questions. Process—convening, deliberating, deciding, documenting—is essential infrastructure.

### F5: Risk Ownership Determines Authority
When authority is contested, "who bears the risk?" often determines who decides. Risk mapping is governance infrastructure.

---

*This is a synthetic environment for structural research. No real organizations, individuals, or decisions are represented.*
