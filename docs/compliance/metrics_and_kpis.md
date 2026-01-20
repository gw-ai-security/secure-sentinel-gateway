# Metrics and KPIs

## Purpose
Define audit-ready KPIs that demonstrate security, compliance, and operational effectiveness.

## KPI table
| KPI name | Purpose | Formula / measurement method | Data source | Target threshold | Owner role | Review frequency |
| --- | --- | --- | --- | --- | --- | --- |
| PII masking effectiveness | Validate sensitive data protection | Masked PII fields / total detected PII fields | Audit logs, redaction reports | >= 98% | AI Security Architect | Monthly |
| Prompt blocking rate | Track unsafe prompt filtering | Blocked prompts / total prompts | Gateway policy logs | 1-5% expected baseline | AI Security Architect | Monthly |
| False positive rate (prompt) | Measure over-blocking risk | False positive cases / total blocked prompts | Review samples, analyst triage notes | <= 2% | AI Security Architect | Monthly |
| False negative rate (prompt) | Measure missed unsafe prompts | Unsafe prompts that passed / total unsafe prompts detected in review | Red team samples, QA reviews | <= 1% | AI Security Architect | Quarterly |
| Response leakage rate | Track data leakage in responses | Leakage incidents / total responses | Audit logs, incident reports | 0 critical incidents | Compliance Officer (Technical) | Monthly |
| Audit log completeness | Validate audit evidence coverage | Logged requests / total requests | Audit log store, gateway counters | >= 99.5% | DevOps Engineer (AWS) | Monthly |
| Time to detect (TTD) | Measure monitoring effectiveness | Median detection time for incidents | Monitoring alerts, incident tickets | <= 15 minutes | DevOps Engineer (AWS) | Monthly |
| Time to respond (TTR) | Measure incident response speed | Median time from detection to containment | Incident tickets, postmortems | <= 4 hours | AI Program and Governance Lead | Quarterly |
| Policy exception rate | Track governance drift | Approved exceptions / total policy checks | Policy exception register | <= 0.5% | Compliance Officer (Organizational) | Quarterly |
| Cost per request | Track operational efficiency | Total gateway cost / total requests | Cloud cost reports, usage logs | <= agreed budget | AI Program and Governance Lead | Monthly |
| LLM provider latency | Track third-party performance | P95 latency per provider | Gateway metrics, provider logs | <= 2s p95 | DevOps Engineer (AWS) | Monthly |
| Evidence freshness | Ensure evidence is current | Evidence artifacts updated within cadence / total artifacts | Audit evidence register | >= 95% | Compliance Officer (Organizational) | Quarterly |

## References
- docs/knowledge_base/risk_ownership_and_escalation.md
- docs/knowledge_base/eu_ai_act_mapping.md
