# Secure Sentinel AI Gateway (SSG)

## Project overview
Secure Sentinel AI Gateway is an enterprise AI gateway that sits between internal systems and large language models. It exists to enforce security controls, protect sensitive data, and provide audit-ready oversight for AI interactions. The project targets organizations that need safe, compliant AI usage without embedding AI risk management into every application.

## Why this project matters
Enterprises face real AI security risks such as prompt injection, data leakage, and uncontrolled model behavior. Regulatory pressure is increasing, including obligations under the EU AI Act. A dedicated AI gateway provides a consistent control point to manage risk, enforce policy, and produce audit evidence across all AI usage.

## What this project demonstrates
- AI architecture skills through clear system boundaries and gateway responsibilities.
- Security-by-design thinking with defined controls for prompt abuse and data protection.
- AWS infrastructure knowledge framed around least privilege, logging, and environment separation.
- EU AI Act compliance coverage across technical and organizational requirements.
- Professional requirements engineering with structured specifications and acceptance criteria.
- Knowledge Base governance as a single source of truth.

## Team-based approach
This project uses a simulated expert team with role-based Codex Skills to mirror real enterprise delivery. Each role contributes defined artifacts and checks, ensuring accountability and traceability across requirements, security, compliance, and documentation.

## Knowledge Base
The Knowledge Base in `docs/knowledge_base/` is the single source of truth. Every phase updates it, and each major decision is traceable to a Knowledge Base entry. This keeps governance, security, and compliance aligned across the team.

## Enterprise Readiness
- Requirements: `docs/requirements/functional_specs.md`, `docs/requirements/system_boundaries_and_non_goals.md`
- Knowledge Base: `docs/knowledge_base/`
- Compliance: `docs/compliance/ai_system_lifecycle.md`, `docs/compliance/metrics_and_kpis.md`, `docs/compliance/third_party_and_llm_risk.md`
- Storyline: `docs/storyline/stakeholder_briefing_pack.md`
- Work reporting: `docs/work_reports/README.md`

## How to Review This Project (Suggested Reading Order)
1. Executive Summary: `docs/storyline/executive_summary.md`
2. Requirements: `docs/requirements/functional_specs.md`, `docs/requirements/system_boundaries_and_non_goals.md`
3. Knowledge Base: `docs/knowledge_base/README.md`
4. Compliance Docs: `docs/compliance/ai_system_lifecycle.md`, `docs/compliance/metrics_and_kpis.md`, `docs/compliance/third_party_and_llm_risk.md`
5. Work Reports: `docs/work_reports/README.md`
6. Storyline: `docs/storyline/stakeholder_briefing_pack.md`

## Project structure explanation
- `app/`: Reserved for future application code; intentionally empty in this phase.
- `docs/`: Core documentation for requirements, compliance, learnings, storyline, and Codex Skills.
- `docs/requirements/`: Requirements engineering artifacts with scope, user stories, and acceptance criteria.
- `docs/compliance/`: Compliance-oriented documentation and control mappings.
- `docs/learnings/`: Learning notes and decision explanations for knowledge transfer.
- `docs/storyline/`: Portfolio narrative artifacts and STAR-based storylines.
- `docs/knowledge_base/`: Single source of truth for decisions, threats, and compliance mappings.
- `docs/skills/`: Role, team, and method skills that define responsibilities and handoffs.
- `infrastructure/`: Reserved for future infrastructure definitions and deployment artifacts.

## Portfolio and interview value
Recruiters can see a documentation-first approach that reflects enterprise AI governance. This repository prepares candidates for roles such as AI architect, AI security architect, compliance officer, and DevOps engineer. It demonstrates structured requirements work, security and compliance thinking, and the ability to communicate clearly across disciplines.
