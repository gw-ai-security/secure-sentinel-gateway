# Architecture Decisions (ADR-Style)

## ADR-00: Phase 0 foundation gate (Go to Phase 1)
- Decision: Confirm Phase 0 completion and authorize Phase 1 entry.
- Rationale: Governance foundations and documentation baselines are in place.
- Consequences: Phase 1 can proceed with requirements formalization and traceability controls.
- Linked requirements: NFR-C1, NFR-C2, NFR-O3.

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

## ADR-03a: Phase 1 entry readiness (Go)
- Decision: Confirm Phase 1 entry readiness following Phase 0 gate completion.
- Rationale: Governance foundations and baseline artifacts meet Phase 1 entry criteria.
- Consequences: Phase 1 work proceeds with requirements formalization and traceability updates.
- Linked requirements: NFR-C1, NFR-C2, NFR-O3.

## ADR-04: Enterprise readiness governance pack
- Decision: Add explicit system boundaries, risk ownership, lifecycle evidence, KPI governance, and third-party risk artifacts.
- Rationale: Enterprise and audit readiness require documented governance beyond baseline requirements.
- Consequences: All roles must reference these artifacts in work reports and traceability updates.
- Linked requirements: NFR-C1, NFR-C2, NFR-C3.

## ADR-05: Risk ownership and escalation model
- Decision: Adopt a category-based risk ownership model with explicit escalation triggers and decision authority.
- Rationale: Audit readiness depends on clear accountability and repeatable escalation paths.
- Consequences: Threats and KPIs must identify owners and escalation thresholds.
- Linked requirements: NFR-O2, NFR-O3.

## ADR-06: Lifecycle evidence expectations
- Decision: Define lifecycle phases with required deliverables and evidence per phase.
- Rationale: EU AI Act readiness requires traceable evidence across the system lifecycle.
- Consequences: Work reports must align to lifecycle evidence requirements.
- Linked requirements: NFR-C2, NFR-C3.

## ADR-07: Third-party LLM risk posture
- Decision: Treat LLM providers and AWS managed services as explicit third-party risk dependencies.
- Rationale: External dependencies materially affect security, compliance, and availability.
- Consequences: Third-party risks must be tracked in compliance and threat documentation.
- Linked requirements: NFR-S1, NFR-S2, NFR-O2.

## ADR-08: Project context handoff snapshots and external feedback capture
- Decision: Maintain timestamped project context handoff snapshots and isolate external chatbot feedback as untrusted input.
- Rationale: Reliable context transfer and auditability require an append-only handoff trail with clear trust boundaries.
- Consequences: Every snapshot must separate facts from assumptions and link to authoritative artifacts; feedback must be reviewed before KB updates.
- Linked requirements: NFR-C1, NFR-C2, NFR-O3.
