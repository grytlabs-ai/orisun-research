# The Evidence Primitive

**What Provenance Looks Like**

---

## Why Evidence Matters

Decisions without evidence are assertions.
Conclusions without provenance are opinions.
Recommendations without sources are guesses.

In governance-grade domains, "trust me" is not acceptable. The chain from input to output must be visible, traceable, and verifiable.

Evidence is not just what you have. It's how you know what you know.

---

## The Evidence Chain

Every output should be traceable through a chain:

```
Claim → Reasoning → Authority → Evidence → Source
```

**Claim:** The statement or recommendation
**Reasoning:** How the claim was derived
**Authority:** What rules or requirements govern
**Evidence:** What facts support the position
**Source:** Where the evidence came from

If any link is missing, the chain breaks. Broken chains are not defensible.

---

## Evidence Types

### Documentary Evidence
Records that exist independent of the decision.

- Contracts and agreements
- Invoices and receipts
- Reports and filings
- Correspondence
- Policies and procedures
- Meeting minutes and resolutions

**Strength:** High (exists independently; verifiable)
**Weakness:** May be incomplete; requires interpretation

### Testimonial Evidence
Statements from individuals with knowledge.

- Interviews
- Declarations
- Certifications
- Attestations

**Strength:** Can fill gaps; provides context
**Weakness:** Subject to bias; memory errors

### Analytical Evidence
Results of examination or analysis.

- Calculations
- Comparisons
- Trend analysis
- Statistical tests

**Strength:** Objective when properly performed
**Weakness:** Depends on input quality; methodology matters

### Observational Evidence
Direct observation of conditions or activities.

- Site visits
- System demonstrations
- Process walkthroughs
- Physical inspection

**Strength:** Direct; not filtered through records
**Weakness:** Point-in-time; limited scope

### Circumstantial Evidence
Facts that support inference.

- Patterns
- Correlations
- Absence of expected records

**Strength:** Can support conclusions when direct evidence unavailable
**Weakness:** Requires careful inference; can mislead

---

## Evidence Attributes

Each piece of evidence should have:

### Identity
- **Evidence ID** — Unique reference
- **Type** — Documentary, testimonial, etc.
- **Description** — What the evidence is

### Source
- **Origin** — Where it came from
- **Provider** — Who provided it
- **Acquisition date** — When obtained
- **Acquisition method** — How obtained

### Reliability
- **Original vs. copy** — Is this the original document?
- **Authentication** — Has authenticity been verified?
- **Completeness** — Is this the full record?
- **Currency** — Is this current or superseded?

### Relevance
- **Subject matter** — What does it pertain to?
- **Time period** — What period does it cover?
- **Parties** — Who does it relate to?
- **Scope** — What decisions does it support?

### Chain of Custody
- **Handling history** — Who has had access?
- **Modifications** — Any changes since acquisition?
- **Storage** — Where is it maintained?

---

## Provenance Requirements

### Complete Traceability
Every claim should trace to evidence. Every piece of evidence should trace to a source.

The question "Where did this come from?" should always have an answer.

### Verifiability
Evidence should be checkable. Another reviewer should be able to:
- Locate the source
- Confirm the evidence exists
- Verify it says what's claimed

### Preservation
Evidence must be preserved for as long as decisions based on it may be reviewed.

- Retention requirements vary by context
- Evidence should not depend on ephemeral sources
- Links should be durable or content should be captured

### Non-Modification
Evidence should not be altered after collection.

- Original state should be preserved
- Any analysis should be separate from the evidence itself
- Versions should be tracked if updates occur

---

## The Evidence Register

A decision system should maintain an evidence register:

| Field | Purpose |
|-------|---------|
| Evidence ID | Unique reference |
| Type | Documentary, testimonial, etc. |
| Description | What it is |
| Source | Where it came from |
| Acquisition date | When obtained |
| Linked decisions | What decisions rely on it |
| Status | Active, superseded, archived |
| Location | Where it's stored |

The register allows:
- Quick retrieval
- Gap identification
- Dependency tracking
- Retention management

---

## Evidence Gaps

When evidence is insufficient, the system should:

1. **Identify the gap** — What evidence is missing?
2. **Specify the requirement** — What would satisfy the need?
3. **Assign accountability** — Who should provide it?
4. **Track resolution** — Has the gap been filled?

**Gap output example:**
```
Evidence Gap: Prior approval documentation

Missing: Written approval from awarding agency for budget modification
Requirement: 2 CFR 200.308 requires prior written approval for budget changes exceeding 10%
Accountability: Program Manager should obtain from Agency Program Officer
Evidence needed: Email approval or formal amendment
```

Gaps are not failures. They are honest assessments of what's known and what isn't.

---

## Evidence vs. Information

Not all information is evidence.

| Information | Evidence |
|-------------|----------|
| Data exists | Data is authenticated |
| Someone said | Statement is documented |
| System shows | Output is traceable |
| Analysis suggests | Methodology is documented |

Evidence has provenance. Information may not.

A system that treats information as evidence is a system that can be wrong without knowing it.

---

## Evidence in AI Systems

AI systems face unique evidence challenges:

### Model Outputs
AI model outputs are not evidence. They are inferences that require:
- Grounding in actual evidence
- Validation by humans
- Traceable reasoning paths

### Generated Content
AI-generated text, summaries, or recommendations should never be treated as primary evidence.

### Source Attribution
When AI cites sources, those citations must be:
- Verifiable (the source actually exists)
- Accurate (the source actually says what's claimed)
- Complete (not selectively quoted)

### Uncertainty
AI systems should explicitly flag:
- Low-confidence conclusions
- Missing evidence
- Conflicting sources

---

## Implementation Note

This document describes **what** evidence handling must support, not **how** to implement it.

Key implementation considerations:
- Evidence must be storable in multiple formats
- Metadata must be captured at acquisition
- Retrieval must be fast and reliable
- Relationships to decisions must be maintained

Specific schema design and storage patterns depend on context and remain outside the scope of this research.

---

*Evidence is not what you believe. It's what you can show.*
