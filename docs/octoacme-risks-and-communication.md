# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- **Support Lead** owns communication with the customer-facing support team; escalates customer-impacting issues to PM and PdM

## Risk Owners by Role

| Risk Category | Primary Owner | Secondary / Consulted |
|---------------|---------------|-----------------------|
| Schedule / delivery | PM | Release Manager |
| Product / scope | PdM | UX Designer, SME |
| Technical / implementation | Developers | PM |
| Customer / support impact | Support Lead | PM, PdM |
| Design / usability | UX Designer | PdM |
| Data / metrics | Data Analyst | PdM, PM |
| Domain / compliance | SME | PdM |
| Release / deployment | Release Manager | Developers, PM |

See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions of each role.

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
