# System Boundaries and Non-Goals

## In-Scope (what SSG does)
- Acts as a policy enforcement gateway between enterprise systems and LLM providers.
- Normalizes requests and responses to enforce consistent security and compliance controls.
- Applies prompt safety checks, data masking, and response filtering at the gateway layer.
- Produces audit-ready logs and evidence artifacts for AI interactions.
- Supports configuration of policies by environment and business unit.

## Out-of-Scope / Non-Goals
- Hosting, training, or fine-tuning LLMs (including model selection or optimization work).
- Building business application logic or end-user interfaces.
- Running real-time model safety research or experimental behavior tuning.
- Managing end-user identity beyond gateway-level authorization checks.
- Providing legal interpretation of regulatory obligations beyond documented mappings.

## Assumptions
1. Enterprise systems integrate with SSG as the single access path to approved LLMs.
2. LLM providers offer contractual and technical controls aligned with enterprise data handling policies.
3. Security and compliance policies are defined outside the gateway and enforced by configuration.
4. Audit logs and evidence artifacts are retained by enterprise policy and accessible for audits.
5. The gateway runs in a controlled AWS environment with standard security services available.

## Known limitations
- Controls are conceptual and policy-driven until implementation artifacts exist.
- Detection efficacy for prompt injection and data leakage depends on model behavior and policy tuning.
- Evidence completeness relies on upstream systems providing accurate identity and context signals.
- Third-party model changes can affect risk posture without immediate gateway changes.

## Trade-offs (intentional)
- Centralized controls prioritize consistency and auditability over per-application customization.
- Provider-agnostic governance favors portability while accepting dependency on external SLAs.
- Documentation-first delivery improves compliance readiness at the cost of deferred implementation detail.

## Risk acceptance statement
SSG does not eliminate all AI-related risks. The project explicitly accepts residual risk from:
- Provider-side model behavior that remains outside gateway control.
- False positives and false negatives in prompt and response screening.
- Latency and availability impacts introduced by external LLM services.
These risks are accepted because the gateway's objective is centralized control, governance, and
auditability rather than model hosting or full model governance.

## References
- docs/requirements/functional_specs.md
- docs/knowledge_base/architecture_decisions.md
- docs/knowledge_base/threat_register.md
- docs/knowledge_base/eu_ai_act_mapping.md
- docs/knowledge_base/risk_ownership_and_escalation.md
