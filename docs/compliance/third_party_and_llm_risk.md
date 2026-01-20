# Third-Party and LLM Risk

## Purpose
Document external dependency risks, assumptions, and mitigations for LLM providers and AWS managed services.

## Dependency map
- LLM providers: OpenAI, AWS Bedrock (conceptual provider integration paths).
- AWS managed services: IAM, CloudWatch, CloudTrail, KMS, VPC, S3, Secrets Manager.

## Data handling assumptions and constraints
- Only approved data classes are sent to external LLMs.
- PII is masked before outbound requests.
- Provider logs do not store customer prompts beyond contractually approved retention.
- Data residency and sub-processor use are governed by enterprise policy.

## Threats unique to external LLM usage
- Model behavior drift affecting safety controls.
- Provider-side logging or telemetry retention outside enterprise control.
- Cross-tenant risk or data leakage due to provider-side faults.
- Service outage or API changes that bypass expected safeguards.
- Latency spikes causing policy bypass or degraded monitoring.

## Contract and policy dependency checklist (non-legal)
- Data processing addendum includes retention limits and deletion rights.
- Sub-processor disclosure and notification requirements are documented.
- Incident notification timelines are contractually defined.
- Audit rights or third-party attestations (SOC 2, ISO 27001) are available.
- Data residency commitments are documented where required.

## Residual risks and mitigations
- Residual risk: Provider-side model issues not detectable by gateway.
  Mitigation: Continuous monitoring, periodic red team testing, diversified provider strategy.
- Residual risk: Third-party outages impacting availability.
  Mitigation: Provider failover plan and operational runbooks.
- Residual risk: Contractual limitations on audit depth.
  Mitigation: Supplement with internal monitoring and evidence collection.

## AWS-specific notes
- IAM: Enforce least privilege for gateway services and LLM access roles.
- Logging: CloudWatch and CloudTrail enabled for gateway actions and configuration changes.
- Encryption: KMS-backed encryption at rest for logs and evidence artifacts.
- Data flow boundaries: VPC egress control and explicit outbound routing to approved providers.

## References
- docs/knowledge_base/threat_register.md
- docs/knowledge_base/eu_ai_act_mapping.md
- docs/requirements/system_boundaries_and_non_goals.md
