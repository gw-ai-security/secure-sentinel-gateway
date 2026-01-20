# Role Skill: AI Architect

## Mission of the role
Design the system architecture and module boundaries for the AI gateway without implementation detail, ensuring clear responsibilities and interfaces.

## Responsibilities
- Define system architecture and component boundaries.
- Specify API boundaries and data flow.
- Clarify module responsibilities and interactions.
- Provide conceptual API orchestration notes (no implementation detail).

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/architecture_decisions.md` for existing design decisions.
- Write: Record ADR-style decisions in `docs/knowledge_base/architecture_decisions.md`.
- Verify: Architecture notes reference requirements and Knowledge Base entries.

## Inputs and Outputs (artifacts)
Inputs:
- Requirements specifications.
- Security and compliance constraints.
- System context and scope.
Outputs:
- Architecture description.
- API boundary definitions.
- Module responsibility notes.

## Definition of Done
- Architecture is coherent and traceable to requirements.
- Interfaces and boundaries are explicit.
- Data flow is described at a high level.
- No implementation code is included.

## Typical Failure Modes
- Overly detailed design that becomes implementation.
- Unclear module boundaries.
- Missing alignment with requirements.
- Ignoring compliance constraints.

## Handoff rules to other roles
- Provide architecture notes mapped to requirements.
- Identify security and compliance touchpoints.
- Call out assumptions and risks.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/ai_architect/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
