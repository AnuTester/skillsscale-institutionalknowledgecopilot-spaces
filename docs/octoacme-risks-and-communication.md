# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with clearly assigned ownership:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner (specific role: e.g., [DevOps Engineer](octoacme-roles-and-personas.md#devops-engineer), [QA Lead](octoacme-roles-and-personas.md#qa-lead))
- Mitigation plan
- Status

## Risk Lifecycle
Clearly defined ownership ensures risks are actively managed:
- **Identify**: All team members during planning and ongoing execution
- **Assess**: Project Manager with input from technical leads (Developers, DevOps, QA Lead)
- **Mitigate**: Assigned Owner executes risk reduction actions and contingency plans
- **Monitor**: Project Manager reviews at weekly syncs; Owners update status
- **Escalate**: Project Manager escalates high-impact risks to Product Lead or Sponsor

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

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
Clear escalation ensures accountability and rapid resolution:
- **Team-level** → **Project Manager** → **Product Lead** → **Sponsor**
- **For security incidents**: Follow the security incident runbook and notify Security on-call immediately
- **For production incidents**: [Release Manager](octoacme-roles-and-personas.md#release-manager) coordinates with [DevOps Engineer](octoacme-roles-and-personas.md#devops-engineer) for immediate response
- **For quality issues**: [QA Lead](octoacme-roles-and-personas.md#qa-lead) escalates to Product Manager with go/no-go recommendation
