# Method Skill: Threat Modeling

## Mission of the role
Apply structured threat modeling to identify AI-specific risks and AWS deployment threats using STRIDE or LINDDUN.

## Responsibilities
- Select and apply STRIDE or LINDDUN.
- Identify AI-specific threats (prompt abuse, data leakage).
- Consider AWS deployment threat vectors.
- Document threats and mitigations at a high level.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/architecture_decisions.md`.
- Write: Register identified threats in `docs/knowledge_base/threat_register.md`.
- Verify: Threats map to at least one security pattern.

## Inputs and Outputs (artifacts)
Inputs:
- System context and architecture notes.
- Security requirements and constraints.
- Deployment environment assumptions.
Outputs:
- Threat list with categories.
- High-level mitigations.
- Assumptions and scope boundaries.

## Definition of Done
- Threats cover AI-specific and deployment risks.
- Each threat has a mitigation concept.
- Assumptions and scope are documented.
- No implementation details are included.

## Typical Failure Modes
- Generic threats without AI-specific focus.
- Missing deployment-specific risks.
- Unclear scope or assumptions.
- Mitigations that are not aligned to risks.

## Handoff rules to other roles
- Provide threat list mapped to requirements.
- Flag critical risks needing design attention.
- Align mitigations with security and compliance roles.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/ai_security_architect/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
