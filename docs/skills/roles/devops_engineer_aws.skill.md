# Role Skill: DevOps Engineer (AWS)

## Mission of the role
Define AWS-native infrastructure decisions and operational safeguards for secure deployment without implementation detail.

## Responsibilities
- Select AWS services and deployment patterns conceptually.
- Apply IAM least privilege principles.
- Define logging, monitoring, and environment separation.
- Specify Docker and Terraform responsibilities.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/architecture_decisions.md` and `docs/knowledge_base/eu_ai_act_mapping.md`.
- Write: Record operational assumptions in `docs/knowledge_base/architecture_decisions.md`.
- Verify: Logging and monitoring requirements are linked to Knowledge Base entries.

## Inputs and Outputs (artifacts)
Inputs:
- Architecture boundaries and data flow.
- Security and compliance requirements.
- Operational constraints.
Outputs:
- Infrastructure decision notes.
- IAM and environment separation guidance.
- Logging and monitoring requirements.

## Definition of Done
- Infrastructure choices align with requirements.
- IAM least privilege is documented.
- Logging and monitoring are defined.
- Environment separation is explicit.

## Typical Failure Modes
- Overly generic infrastructure guidance.
- Missing or weak IAM considerations.
- Logging and monitoring gaps.
- Mixing environments or unclear separation.

## Handoff rules to other roles
- Provide infrastructure notes mapped to requirements.
- Identify operational risks and constraints.
- Align with compliance logging needs.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/devops_engineer_aws/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
