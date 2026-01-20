# Work Reporting Standard

## Purpose
Work reports provide auditability, workload tracking, and stakeholder-ready status updates. They document what was done, why it matters, and how it links to project artifacts and the Knowledge Base.

## Mandatory rule
No task is Done until the work report is updated.

## Where to write
- Primary location: `docs/work_reports/roles/<role>/phase_<N>.md`
- Optional consolidated view: `docs/work_reports/phases/phase_<N>/overview.md`

## Naming convention
- Role reports: `docs/work_reports/roles/<role>/phase_<N>.md`
- Phases range from `phase_0` to `phase_4` only.

## Timestamp format
Use exactly: `YYYY-MM-DD HH:MM Europe/Vienna`

## Work report entry template
```
- Timestamp: YYYY-MM-DD HH:MM Europe/Vienna
  Role: <role name>
  Phase: phase_<N>
  Work package: <short description>
  Decisions: <key decisions or rationale>
  Artifacts updated:
  - <path to file>
  - <path to file>
  Knowledge Base updates:
  - <path to KB file>
  Cross-links:
  - <path to related requirement or compliance doc>
```

## Cross-link rules
- Link every entry to created or updated artifacts.
- Link to any Knowledge Base update for the same work package.
- Reference requirements or compliance artifacts when applicable.
