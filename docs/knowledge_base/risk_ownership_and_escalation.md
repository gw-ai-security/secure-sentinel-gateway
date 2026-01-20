# Risk Ownership and Escalation

## Purpose
Define clear ownership, escalation, and decision authority for AI gateway risks to support audit readiness.

## Risk ownership by category
| Risk category | Primary owner role | Backup owner | Decision authority | Escalation path |
| --- | --- | --- | --- | --- |
| Security | AI Security Architect | DevOps Engineer (AWS) | AI Program and Governance Lead | Security incident lead -> AI Program and Governance Lead -> Compliance Officer (Organizational) |
| Compliance | Compliance Officer (Organizational) | Compliance Officer (Technical) | AI Program and Governance Lead | Compliance Officer (Organizational) -> Legal/Policy (external) -> Executive sponsor |
| Operational | DevOps Engineer (AWS) | AI Architect | AI Program and Governance Lead | On-call lead -> DevOps Manager -> AI Program and Governance Lead |
| Third-party | AI Program and Governance Lead | Compliance Officer (Organizational) | Executive sponsor | Vendor manager -> AI Program and Governance Lead -> Executive sponsor |
| Reputational | AI Program and Governance Lead | Compliance Officer (Organizational) | Executive sponsor | Communications lead -> AI Program and Governance Lead -> Executive sponsor |

## Escalation triggers (mandatory)
- Security: PII exposure confirmed, repeated prompt injection events, or failed audit log integrity checks.
- Compliance: Evidence gaps in audits, regulatory inquiry, or policy exceptions that exceed threshold.
- Operational: SLA breach, prolonged outage, or monitoring gaps beyond agreed limits.
- Third-party: Provider incident affecting data handling, material contract change, or sub-processor addition.
- Reputational: Customer-impacting AI incident or public disclosure risk.

## Decision authority for risk acceptance
- Routine risk acceptance: AI Program and Governance Lead.
- High-impact risk acceptance: Executive sponsor with Compliance Officer (Organizational) concurrence.
- Emergency acceptance: Incident commander, with retrospective approval within 5 business days.

## References
- docs/knowledge_base/threat_register.md
- docs/knowledge_base/eu_ai_act_mapping.md
- docs/knowledge_base/architecture_decisions.md
