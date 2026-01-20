# Team Skill: Team Orchestration

## Mission of the role
Ensure the project advances in a controlled, phase-based manner with clear role switching, review gates, and mandatory Knowledge Base updates.

## Responsibilities
- Define phase order and entry/exit criteria.
- Enforce role separation and review checkpoints.
- Require Knowledge Base updates at the end of each phase.
- Resolve sequencing conflicts across roles.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/README.md` to enforce update rules.
- Write: Record phase gate decisions in `docs/knowledge_base/architecture_decisions.md`.
- Verify: Each phase updates at least one Knowledge Base file.

## Inputs and Outputs (artifacts)
Inputs:
- Project charter and task list.
- Outputs from role skills.
- Definition of Done criteria per phase.
Outputs:
- Phase plan and gate decisions.
- Role assignment notes.
- Completion checklist per phase.

## Definition of Done
- All phases are executed in the prescribed order.
- Each phase has a documented gate decision.
- Required artifacts are present and complete.
- Knowledge Base updates are confirmed for each phase.

## Done Gate (Phase Completion)
- Required artifacts are created or updated.
- Every contributing role has written a work report entry in its `phase_<N>.md` file.
- The Knowledge Base Curator confirms required Knowledge Base references exist.

## Enterprise Readiness Gate (Checklist)
- System boundaries and non-goals documented in `docs/requirements/system_boundaries_and_non_goals.md`.
- Risk ownership and escalation recorded in `docs/knowledge_base/risk_ownership_and_escalation.md`.
- Lifecycle evidence defined in `docs/compliance/ai_system_lifecycle.md`.
- KPI governance documented in `docs/compliance/metrics_and_kpis.md`.
- Third-party risk posture documented in `docs/compliance/third_party_and_llm_risk.md`.
- Stakeholder briefing pack updated in `docs/storyline/stakeholder_briefing_pack.md`.

## Typical Failure Modes
- Parallel work without coordination causing gaps.
- Missing review gates or unchecked deliverables.
- Role conflation that hides accountability.
- Knowledge Base updates skipped or inconsistent.

## Handoff rules to other roles
- Handoff only after phase gate is approved.
- Provide a concise checklist of completed artifacts.
- Call out any open risks or dependencies.

## Work Reporting (Mandatory)
- After completing any work package or phase task, update:
  docs/work_reports/roles/ai_program_governance_lead/phase_<N>.md
- Add a new entry using the official template from docs/work_reports/README.md
- Link to:
  - all created/updated artifacts (files)
  - any Knowledge Base updates (docs/knowledge_base/...)
- The task is NOT considered done until this report entry exists.
