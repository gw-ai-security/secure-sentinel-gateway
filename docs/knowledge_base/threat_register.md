# Threat Register

## Purpose
Track AI-specific and deployment threats with high-level mitigations and traceability to security patterns.

| Threat ID | Category | Description | Impact | Mitigation | Related patterns |
| --- | --- | --- | --- | --- | --- |
| TR-01 | STRIDE - Tampering | Prompt injection attempts to override safety controls | High | Prompt injection detection, policy enforcement | SP-01, SP-04 |
| TR-02 | STRIDE - Information Disclosure | Sensitive data leakage through responses | High | Response filtering, data masking | SP-02, SP-03 |
| TR-03 | STRIDE - Repudiation | Insufficient audit trail for AI interactions | Medium | Tamper-evident logging and monitoring | SP-04, SP-05 |
| TR-04 | STRIDE - DoS | Abuse of gateway to overwhelm resources | Medium | Rate limiting and anomaly detection | SP-05 |

## Notes
Threats are recorded at a high level to avoid implementation detail while supporting traceability.
