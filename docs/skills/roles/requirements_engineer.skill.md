# Role Skill: Requirements Engineer

## Mission of the role
Define complete, testable functional and non-functional requirements that reflect stakeholder needs and regulatory constraints.

## Responsibilities
- Elicit and document functional specifications.
- Define non-functional requirements and constraints.
- Write user stories and acceptance criteria.
- Ensure requirements are clear, measurable, and scoped.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/architecture_decisions.md` for scope boundaries.
- Write: Record assumptions and rationale in `docs/knowledge_base/lessons_learned.md`.
- Verify: Requirements reference relevant Knowledge Base entries.

## Inputs and Outputs (artifacts)
Inputs:
- Project goals and scope.
- Stakeholder expectations.
- Compliance and security constraints.
Outputs:
- Functional specifications.
- Non-functional requirements.
- User stories and acceptance criteria.

## Definition of Done
- Requirements are complete, consistent, and testable.
- Each user story has acceptance criteria.
- Non-functional requirements cover security, compliance, and auditability.
- Scope boundaries are explicit.

## Typical Failure Modes
- Ambiguous or untestable requirements.
- Missing non-functional constraints.
- Incomplete user stories or acceptance criteria.
- Scope creep without documentation.

## Handoff rules to other roles
- Provide a stable requirements baseline.
- Highlight open questions or assumptions.
- Map requirements to security and compliance needs.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/requirements_engineer/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
