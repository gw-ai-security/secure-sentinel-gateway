---
name: project-context-handoff
description: Create project context handoff snapshots and capture external chatbot feedback with timestamped files for Secure Sentinel AI Gateway (SSG); use when transferring context, before external chatbot queries, after session changes, or at phase gates.
---
# Team Skill: Project Context Handoff

## Mission
Create a single, copy-paste-ready Project Context Handoff snapshot that captures the current repository truth so another AI chatbot can immediately understand the project context. Capture external chatbot responses separately as untrusted feedback with timestamps.

## Responsibilities
- Produce authoritative handoff snapshots from repository artifacts only.
- Maintain an append-only history of snapshots and feedback files.
- Separate facts from assumptions explicitly.
- Record external chatbot feedback as untrusted input only.
- Link to key repository documents for traceability.

## Knowledge Base interaction (read/write duties)
- Read: `docs/knowledge_base/*`, `docs/requirements/*`, `docs/compliance/*`, `docs/storyline/*`, `docs/work_reports/*`, `README.md`.
- Write: `docs/knowledge_base/architecture_decisions.md` when handoff governance or process changes.
- Verify: Each snapshot references the Knowledge Base as the single source of truth.

## Inputs and Outputs (artifacts)
Inputs:
- Current repository documentation under `docs/` and `README.md`.
Outputs:
- Snapshot: `docs/handoff/snapshots/YYYY-MM-DD_HHMM_Europe-Vienna_project_context_handoff.md`
- Feedback (optional): `docs/handoff/feedback/YYYY-MM-DD_HHMM_Europe-Vienna_external_feedback.md`

## Folder Structure (required)
```
docs/handoff/
├── README.md
├── snapshots/
└── feedback/
```

## Timestamp and Naming
- Use Europe/Vienna time.
- Snapshot: `YYYY-MM-DD_HHMM_Europe-Vienna_project_context_handoff.md`
- Feedback: `YYYY-MM-DD_HHMM_Europe-Vienna_external_feedback.md`

## Templates (required)
- Snapshot template: `docs/handoff/snapshots/<timestamp>_project_context_handoff.md`
- Feedback template: `docs/handoff/feedback/<timestamp>_external_feedback.md`

## Workflow Integration (when and who)
- Use this skill:
  1) At the end of every session (snapshot per session is mandatory).
  2) If a session makes no documentation changes, still create a snapshot and note "No repo changes" in the Change Log section.
  2) Before sending context to an external chatbot.
  3) After a phase gate decision or readiness review.
  4) Before stakeholder review or interview simulation.
- Ownership:
  - Snapshot owner: role leading the current session (default: AI Program and Governance Lead).
  - Required updaters: Snapshot owner creates the handoff; reviewers capture feedback in `docs/handoff/feedback/` when external input is used.
  - Reviewers for feedback: AI Architect, AI Security Architect, Compliance Officer (EU AI Act), Program/Governance Lead.
- Link snapshots to work reports for the current phase in `docs/work_reports/roles/<role>/phase_<N>.md`.

## Definition of Done
A snapshot is done only if it includes:
- Project summary and current phase/status.
- Clear separation of facts vs assumptions.
- Links to key artifacts (relative paths).
- Current decisions or ADR references.
- Security and compliance summary.
- Open questions and next actions.
- Change log since last snapshot (if one exists).
- Owner and timestamp.

Feedback is done only if it includes:
- Provenance (tool, model if known, purpose).
- Input snapshot reference.
- Untrusted content warning.
- Review ownership and decision log.

## Typical Failure Modes
- Invented project state not grounded in repository artifacts.
- External feedback mixed into authoritative KB without review.
- Missing timestamps or incorrect file naming.
- Missing traceability links to key documents.

## Work Reporting (Mandatory)
- After creating a snapshot or feedback file, update:
  `docs/work_reports/roles/ai_program_governance_lead/phase_<N>.md`
- Add a new entry using the official template from `docs/work_reports/README.md`.
- Link to created artifacts and Knowledge Base updates.
