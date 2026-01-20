# Threat Register

## Purpose
Track AI-specific and deployment threats with high-level mitigations, owners, and lifecycle traceability.

| Threat ID | Category | Description | Impact | Mitigation | Owner | Lifecycle phase | Related patterns |
| --- | --- | --- | --- | --- | --- | --- | --- |
| TR-01 | STRIDE - Tampering | Prompt injection attempts to override safety controls | High | Prompt injection detection, policy enforcement | AI Security Architect | Build, Operate | SP-01, SP-04 |
| TR-02 | STRIDE - Information Disclosure | Sensitive data leakage through responses | High | Response filtering, data masking | AI Security Architect | Operate, Monitor | SP-02, SP-03 |
| TR-03 | STRIDE - Repudiation | Insufficient audit trail for AI interactions | Medium | Tamper-evident logging and monitoring | DevOps Engineer (AWS) | Operate, Monitor | SP-04, SP-05 |
| TR-04 | STRIDE - DoS | Abuse of gateway to overwhelm resources | Medium | Rate limiting and anomaly detection | DevOps Engineer (AWS) | Operate, Monitor | SP-05 |
| TR-05 | Third-party | Provider-side data retention beyond policy | High | Contract constraints, periodic provider reviews | Compliance Officer (Organizational) | Design, Operate | SP-02 |
| TR-06 | Third-party | LLM provider outage or API change impacting availability | Medium | Provider failover plan, runbooks | DevOps Engineer (AWS) | Deploy, Operate | SP-05 |
| TR-07 | Compliance | Evidence gaps in logs or audit artifacts | High | Evidence register, retention checks | Compliance Officer (Organizational) | Monitor, Change | SP-04 |
| TR-08 | Operational | Unauthorized configuration change in gateway policies | Medium | Change management approvals, logging | AI Program and Governance Lead | Change | SP-04 |

## Notes
Threats are recorded at a high level to avoid implementation detail while supporting traceability.
