# EU AI Act Technical Controls - High-Level Mapping

## Purpose
Document technical safeguards for the Secure Sentinel AI Gateway and map them to EU AI Act obligations at a high level to support audit readiness.

## Control mappings (high-level)
| Control area | Description | Related requirements | EU AI Act obligation (high-level) | Evidence artifacts |
| --- | --- | --- | --- | --- |
| Risk management | Identify, assess, and review AI risks at the gateway level | FR-3, FR-4, FR-5, NFR-O2 | Risk management system | Risk review notes, risk register summary |
| Data protection | Mask and minimize sensitive data before model interaction | FR-4, NFR-S1 | Data governance and protection | Data masking policy, sample audit logs |
| Security controls | Detect prompt injection and unsafe requests | FR-3, FR-5 | Cybersecurity and robustness | Prompt safety policy, test scenarios |
| Logging and monitoring | Maintain tamper-evident logs and alerts | FR-6, FR-10, NFR-C1, NFR-O2 | Logging, monitoring, and incident response | Audit log retention policy, monitoring dashboards |
| Transparency and traceability | Ensure requests and responses are traceable | FR-6, NFR-C2, NFR-O3 | Technical documentation and traceability | Traceability notes, change logs |

## Notes
- This mapping is intentionally high-level and intended for documentation-first planning.
- Detailed legal interpretation is out of scope and should be verified by legal counsel.
