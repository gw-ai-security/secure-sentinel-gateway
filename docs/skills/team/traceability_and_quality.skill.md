# Team Skill: Traceability and Quality

## Mission of the role
Maintain end-to-end traceability between requirements, architecture, security, and compliance with clear Definition of Done and auditable evidence in the Knowledge Base.

## Responsibilities
- Define traceability links across artifacts.
- Establish Definition of Done per phase.
- Require evidence and audit artifacts.
- Verify quality checks before handoff.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/eu_ai_act_mapping.md`, `docs/knowledge_base/security_patterns.md`, `docs/knowledge_base/threat_register.md`.
- Write: Update traceability notes in `docs/knowledge_base/architecture_decisions.md`.
- Verify: Each requirement is linked to at least one Knowledge Base entry.

## Inputs and Outputs (artifacts)
Inputs:
- Requirements specifications.
- Architecture and security notes.
- Compliance mappings and controls.
Outputs:
- Traceability matrix or mapping notes.
- Phase Definition of Done criteria.
- Audit evidence checklist.

## Definition of Done
- Every requirement maps to an architecture and security consideration.
- Compliance controls are linked to requirements.
- Evidence artifacts are identified and referenced.
- Traceability is documented and reviewable in the Knowledge Base.

## Typical Failure Modes
- Requirements without mapped controls.
- Missing evidence or audit artifacts.
- Inconsistent Definition of Done across phases.
- Unverifiable claims about compliance.

## Handoff rules to other roles
- Provide traceability notes with every artifact.
- Flag any unmapped items explicitly.
- Require confirmation of evidence ownership.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/knowledge_base_curator/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
