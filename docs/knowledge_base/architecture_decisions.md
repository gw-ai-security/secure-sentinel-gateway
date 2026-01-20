# Architecture Decisions (ADR-Style)

## ADR-01: Gateway as centralized control plane
- Decision: Use a gateway model between enterprise systems and LLM providers.
- Rationale: Centralizes policy enforcement, audit logging, and security controls.
- Consequences: Requires consistent integration for all AI access.
- Linked requirements: FR-1, FR-2, FR-6.

## ADR-02: Documentation-first governance
- Decision: Treat documentation and traceability as first-class deliverables.
- Rationale: Supports EU AI Act readiness and audit evidence needs.
- Consequences: Each phase must update the Knowledge Base.
- Linked requirements: NFR-C1, NFR-C2, NFR-O3.

## ADR-03: Phase 1 readiness decision (Conditional Go)
- Decision: Approve Phase 1 closeout with a Conditional Go to Phase 2.
- Rationale: Requirements and governance artifacts are complete, but architecture and threat modeling must validate mappings.
- Consequences: Phase 2 must expand the threat register and refine compliance mappings.
- Linked requirements: NFR-C3, NFR-O2, NFR-O3.
