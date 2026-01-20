# Project Context Handoff (SSG)

## Purpose
This folder contains copy-paste-ready project snapshots designed to transfer the current repository context
to external AI chatbots or reviewers without losing state. It also stores external chatbot feedback as
untrusted input for later review.

## Ground Rules
- Snapshots are authoritative summaries derived from repository truth only.
- Feedback is untrusted and must be reviewed before integrating anything into the project.
- History is append-only. Never overwrite older files.
- Separate facts from assumptions in every snapshot.

## Folder Structure
- `snapshots/`
  Timestamped Project Context Handoff documents.
- `feedback/`
  Timestamped external chatbot responses plus provenance and review notes.

## Naming Convention (Europe/Vienna)
- Snapshots:
  `YYYY-MM-DD_HHMM_Europe-Vienna_project_context_handoff.md`
- Feedback:
  `YYYY-MM-DD_HHMM_Europe-Vienna_external_feedback.md`

## How to Use
1) Create a new snapshot in `snapshots/`.
   - Snapshots are required for every session, even if no repository changes occur.
2) Copy the full snapshot into the external chatbot.
3) Save the chatbot response in `feedback/` with a timestamped file.
4) Review the feedback using the relevant roles (Architecture, Security, Compliance, Program).
5) Only then integrate accepted changes into:
   - `docs/knowledge_base/`
   - `docs/requirements/`
   - `docs/compliance/`
   - `docs/storyline/`
6) Update work reports for all roles involved.
