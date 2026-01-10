# Synthetic Organization: Alpha-Stable

**Archetype: Stable Ontology Environment**

---

## Purpose

This synthetic organization exhibits properties of a **stable ontology environment**:
- Terms have fixed meanings over time
- Roles are clearly defined
- Decisions follow established procedures
- Authority structures are unambiguous

It serves as a **baseline** for understanding minimum infrastructure requirements.

---

## Entity Profile

| Attribute | Value |
|-----------|-------|
| Entity ID | alpha-001 |
| Entity Type | Local Government |
| Subtype | Municipality |
| Size Class | Medium (50-250 employees) |
| Geographic Scope | Single jurisdiction |
| Primary Domain | Public services |

---

## Role Structure

| Role | Authority Level | Decision Types |
|------|-----------------|----------------|
| Executive | Full (within policy) | Strategic, budget, personnel |
| Department Head | Delegated (within department) | Operational, procurement under threshold |
| Program Manager | Limited (within program) | Activity, vendor selection under threshold |
| Specialist | Advisory | Recommendations only |

---

## Authority Structure

### Hierarchy
```
Federal Requirements
└── State Requirements
    └── Local Ordinances
        └── Administrative Policies
            └── Departmental Procedures
                └── Program Guidelines
```

### Resolution Rule
Higher authority governs. Conflicts resolved by escalation to level that has authority over both provisions.

---

## Decision Type Catalog

### Type D1: Cost Allowability
- **Question pattern:** "Is [cost] allowable under [award]?"
- **Required context:** Award ID, cost category, amount, timing
- **Authority path:** Award terms → Regulations → Statute
- **Decision owner:** Program Manager (under threshold), Department Head (over threshold)

### Type D2: Prior Approval
- **Question pattern:** "Does [action] require prior approval?"
- **Required context:** Action type, award ID, threshold status
- **Authority path:** Award terms → Regulations
- **Decision owner:** Program Manager (identification), Agency (approval)

### Type D3: Procurement Method
- **Question pattern:** "What procurement method applies to [purchase]?"
- **Required context:** Estimated value, nature of goods/services, competition availability
- **Authority path:** Local policy → State law → Federal regulations
- **Decision owner:** Procurement Officer

---

## Example Decision Scenarios

### Scenario D1-01: Travel Cost
```
Question: Is the proposed conference registration allowable?

Context:
- Award: Grant FY24-0123
- Cost: $450 conference registration
- Purpose: Professional development related to grant activities
- Timing: Month 8 of 24-month award

Authority Chain:
- 2 CFR 200.474: Training and education costs allowable if related to grant
- Award Terms: No special conditions on training
- Entity Policy: Pre-approval required for travel over $500

Decision:
- Outcome: Allowable
- Conditions: None (under policy threshold)
- Rationale: Direct benefit to grant; within cost principles; no approval needed

Decision Record: D1-01-20240115
Decision Maker: Program Manager
```

### Scenario D2-01: Budget Modification
```
Question: Does transferring $12,000 from Personnel to Equipment require prior approval?

Context:
- Award: Grant FY24-0123
- Total award: $150,000
- Transfer amount: $12,000 (8% of total)
- Categories: Personnel to Equipment

Authority Chain:
- 2 CFR 200.308: Prior approval required for budget changes >10% of total
- Award Terms: Standard terms apply

Analysis:
- 8% is under the 10% threshold
- Transfer is between standard categories
- No special conditions triggered

Decision:
- Outcome: Prior approval NOT required
- Conditions: Document rationale in file
- Rationale: Within automatic transfer authority

Decision Record: D2-01-20240122
Decision Maker: Program Manager
```

---

## Observations (Structural)

### What Works in Stable Environments

1. **Simple authority resolution** — Clear hierarchy means unambiguous precedence
2. **Predictable decision paths** — Same question type follows same route
3. **Role clarity** — Authority levels are obvious
4. **Threshold-based automation** — Many decisions can be rule-governed

### Infrastructure Requirements (Minimum)

| Requirement | Rationale |
|-------------|-----------|
| Authority hierarchy storage | Must traverse from decision to governing authority |
| Role-based routing | Decisions must reach appropriate authority level |
| Threshold detection | Automated identification of approval requirements |
| Decision record capture | Minimum provenance for audit |

### What This Archetype Does NOT Test

- Semantic drift (terms changing meaning)
- Authority conflicts (competing requirements)
- Interpretive ambiguity
- Multi-stakeholder governance

These require Archetypes B and C.

---

## Findings

### F1: Baseline is Simple
In stable ontology environments, decision infrastructure requirements are minimal. The challenge is capture, not resolution.

### F2: Rules Suffice (Mostly)
When authority is clear and context is stable, rule-based systems can handle most decisions. AI adds value at edges, not core.

### F3: The Trap of Assuming Stability
Many organizations believe they operate in Alpha-Stable conditions when they don't. The infrastructure must support fluidity even when it's not immediately needed.

---

*This is a synthetic environment for structural research. No real organizations, individuals, or decisions are represented.*
