# Architecture Overview (Conceptual)

## Purpose
Provide a recruiter-friendly, high-level view of the Secure Sentinel AI Gateway without implementation detail.

## Conceptual components
- Enterprise clients: Internal applications and users that submit AI requests.
- Gateway control plane: Policy enforcement, request normalization, and response filtering.
- Security controls: Prompt safety checks, data masking, and abuse detection at the gateway.
- Compliance controls: Audit logging, evidence capture, and policy exception tracking.
- LLM providers: Approved external or internal model endpoints.

## Conceptual request/response flow
1. Enterprise clients submit requests to the gateway.
2. The gateway authenticates, authorizes, and applies policy checks.
3. Sensitive data is masked before outbound requests to LLM providers.
4. LLM responses return through the gateway for response filtering.
5. Audit logs and evidence artifacts are captured for governance review.

## Control placement
- Security controls sit at the gateway to prevent prompt abuse and data leakage.
- Compliance controls sit at the gateway to ensure audit-ready logging and traceability.
- Governance controls sit in documentation and work reporting to enforce accountability.

## Scope statement
This is a conceptual architecture intended to orient stakeholders; it is not a full technical design.

## References
- docs/requirements/functional_specs.md
- docs/requirements/system_boundaries_and_non_goals.md
- docs/knowledge_base/architecture_decisions.md
