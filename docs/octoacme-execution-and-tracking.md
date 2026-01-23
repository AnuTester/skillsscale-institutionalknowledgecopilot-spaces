# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Key Roles in Execution
- **[Developers](octoacme-roles-and-personas.md#developers)**: Build and test features, participate in reviews
- **[QA Lead](octoacme-roles-and-personas.md#qa-lead)**: Define test strategies and ensure quality gates are met
- **[Project Manager](octoacme-roles-and-personas.md#project-managers)**: Track progress, manage risks and dependencies
- **[Product Manager](octoacme-roles-and-personas.md#product-managers)**: Clarify requirements and prioritize work
- **[UX Designer](octoacme-roles-and-personas.md#ux-designer)**: Validate design implementation and user experience quality
- **[DevOps Engineer](octoacme-roles-and-personas.md#devops-engineer)**: Ensure CI/CD pipelines function properly and infrastructure is ready

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - **Developers**: Create small PRs (<= 400 lines when possible)
  - **Developers**: Include issue link and acceptance criteria in PR description
  - **Developers**: Run automated tests and linting in CI before requesting review
  - **Developers**: Obtain at least one approval before merging (or team-defined policy)
  - **QA Lead**: Validate that PR meets quality standards before final approval

## Quality & Testing
- **Developers**: Write unit tests for new logic
- **Developers**: Create integration tests where applicable
- **QA Lead**: Define and execute end-to-end smoke tests for critical flows before release
- **DevOps Engineer**: Configure security scanning in CI
- **QA Lead**: Coordinate manual QA for feature acceptance when needed
- **QA Lead**: Sign off on quality gates before promoting to production

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
Clear escalation paths ensure issues are resolved quickly with appropriate stakeholder involvement:
- **Level 1**: Team-level triage in daily standup (Developers, QA Lead)
- **Level 2**: Project Manager escalates to Product Lead and dependent teams
- **Level 3**: Project Manager coordinates sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] **Developers**: Branching and PR conventions documented in repo
- [ ] **DevOps Engineer**: CI configured for tests and lint
- [ ] **Project Manager**: Regular demos scheduled with stakeholders
- [ ] **Project Manager**: Risk register updated weekly
- [ ] **QA Lead**: Test plan and quality gates documented
- [ ] **QA Lead**: QA handoff process defined for feature acceptance
- [ ] **UX Designer**: Design validation checkpoints established with developers
- [ ] **Release Manager**: Release readiness criteria communicated to team
