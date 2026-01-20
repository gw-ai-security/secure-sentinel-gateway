# Role Skill: Compliance Officer (EU AI Act, Technical)

## Mission of the role
Define technical safeguards required by the EU AI Act, focusing on monitoring, logging, risk management, and control mapping.

## Responsibilities
- Identify technical safeguards aligned to EU AI Act obligations.
- Specify logging, monitoring, and risk scoring needs.
- Map controls to relevant EU AI Act articles.
- Ensure evidence requirements are clear.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/eu_ai_act_mapping.md`, `docs/knowledge_base/threat_register.md`, `docs/knowledge_base/risk_ownership_and_escalation.md`.
- Write: Maintain compliance mappings in `docs/knowledge_base/eu_ai_act_mapping.md`.
- Verify: Technical controls link to requirements and Knowledge Base entries.

## Inputs and Outputs (artifacts)
Inputs:
- Requirements and system context.
- Architecture and security notes.
- EU AI Act references.
Outputs:
- Technical safeguards list.
- Control-to-article mappings.
- Evidence and audit expectations.
- Lifecycle, KPI, and third-party risk alignment notes.

## Definition of Done
- Technical controls are mapped to EU AI Act obligations.
- Logging and monitoring requirements are explicit.
- Risk scoring approach is defined at a high level.
- Evidence requirements are documented.

## Typical Failure Modes
- Controls listed without article linkage.
- Missing evidence expectations.
- Overlooking monitoring or incident response needs.
- Vague or untestable control descriptions.

## Handoff rules to other roles
- Provide control mappings with references.
- Call out any compliance gaps or risks.
- Align with organizational compliance inputs.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/compliance_officer_eu_ai_act_technical/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
