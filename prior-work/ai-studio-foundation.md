# Prior Work: Cam's AI Studio

**Foundation Research from October 2025**

---

## Overview

Before the current decision intelligence infrastructure work, foundational research was conducted to map the AI ecosystem through a governance lens.

This work produced:
- A structured catalog of 97 tools across 6 workspaces
- Visual frameworks for understanding ontology-aware vs. vector-centric design paths
- An audit-informed methodology for AI system design

---

## The AI Studio Framework

The AI Studio organizes the AI ecosystem into six creative workspaces:

| Workspace | Function | Tool Count |
|-----------|----------|------------|
| **Data Bench** | Sources & Stewardship | 15 |
| **Preparation Bay** | Cleaning & Structuring | 16 |
| **Model Workshop** | Exploration & Prototyping | 15 |
| **Storage Cellar** | Indexes & Caches | 14 |
| **Operations Hub** | Pipelines & Delivery | 23 |
| **Governance Loft** | Evaluation & Controls | 14 |

Each workspace corresponds to a function in the AI development lifecycle, with explicit attention to governance and controls throughout.

---

## Key Insight: Ontology-Aware vs. Vector-Centric Paths

The research identified two primary design paths depending on ontology maturity:

**Ontology-Aware Path (37 tools)**
- When: Knowledge graph and ontology are mature
- Approach: Structured querying (SPARQL/graph), minimal brute-force vector search
- Categories: Knowledge graph (RDF), ontology alignment, provenance & metadata, vocabulary alignment

**Vector-Centric Path (60 tools)**
- When: Ontology is absent or partial
- Approach: Embeddings, RAG pipelines, robust evaluation
- Categories: Embeddings, vector DB, serving, acceleration, open models

**Design Heuristic:** Always close the loop with evaluation + observability + provenance, regardless of path.

---

## Interactive Visualization

The complete AI Studio ecosystem is visualized in an interactive Flourish chart:

**[Cam's AI Studio - Interactive Visualization](https://public.flourish.studio/visualisation/25694650/)**

This visualization shows:
- All 97 cataloged tools
- Distribution across workspaces
- Ontology-aware vs. vector-centric classification
- Maturity indicators (Stable OSS, Active, Mature, Emerging)

---

## Publication

The methodology and findings were published in October 2025:

**"From Audit to AI: Building a Defensible Foundation for Applied Intelligence"**

*Cam Smith, CIA | Founder + Principal Consultant, DC Smith Advisory*

Key themes:
- Audit mindset applied to AI research (criteria → evidence → conclusion)
- Risk-based decision heuristics (Greenlight / Governed Pilot / Restricted / Decline)
- Safe-by-design principles (method over magic, evidence over vibes, human accountability)
- Pace layering for responsible deployment

The article established the foundation for later work on decision intelligence infrastructure, demonstrating early thinking about:
- Ontology-first design
- Governance as primitive
- Human-in-the-loop as non-negotiable
- Evidence and provenance requirements

---

## Connection to Current Work

The AI Studio research informed the current decision intelligence infrastructure in several ways:

| AI Studio Insight | Current Infrastructure |
|-------------------|----------------------|
| Ontology maturity determines design path | Bounded reasoning planes with defined ontological scope |
| Governance must be designed in, not bolted on | Authority anchoring as primitive |
| Evidence and provenance are non-negotiable | Decision provenance by default |
| Human accountability stays put | First-class refusal; AI assists, never replaces |

The journey from tool cataloging to substrate architecture reflects the evolution from "what tools exist" to "what infrastructure is missing."

---

## Data Availability

The underlying Cam's AI Studio Catalog 2025 (Enhanced) contains:
- 97 tools with full metadata
- Workspace classification
- Category assignment
- Ontology-aware vs. vector-centric designation
- Maturity indicators
- Design heuristic alignment

For access to the underlying data or methodology details, contact: hello@dcsmithadvisory.com

---

*This prior work established the audit-informed lens that shaped all subsequent infrastructure research.*
