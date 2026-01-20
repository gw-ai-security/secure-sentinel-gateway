# Role Skill: Data Engineer

## Mission of the role
Define data flow, retrieval, and knowledge base concepts for AI safety and context retrieval without implementation detail.

## Responsibilities
- Describe vector database and RAG concepts.
- Define knowledge base scope for malicious patterns.
- Document data flow and retrieval policies.
- Clarify data retention and access boundaries.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/security_patterns.md` and `docs/knowledge_base/threat_register.md`.
- Write: Prepare Knowledge Base content for future retrieval in `docs/knowledge_base/lessons_learned.md`.
- Verify: Data classification and update rules are documented in the Knowledge Base.

## Inputs and Outputs (artifacts)
Inputs:
- System requirements and context.
- Security constraints.
- Compliance guidelines.
Outputs:
- Data flow descriptions.
- Retrieval and policy notes.
- Knowledge base scope definition.

## Definition of Done
- Data flow is clear and consistent with architecture.
- Retrieval policies align with security requirements.
- Knowledge base scope is defined and justified.
- Data access boundaries are documented.

## Typical Failure Modes
- Vague or undefined data boundaries.
- Retrieval policies that conflict with security.
- Unclear ownership or provenance of data.
- Missing consideration of retention or deletion.

## Handoff rules to other roles
- Provide data flow notes tied to requirements.
- Highlight data risks and mitigations.
- Align with compliance expectations.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/data_engineer/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
