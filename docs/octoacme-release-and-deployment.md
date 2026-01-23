# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Key Roles
- **[Release Manager](octoacme-roles-and-personas.md#release-manager)**: Coordinates release planning, schedules, and communications
- **[DevOps Engineer](octoacme-roles-and-personas.md#devops-engineer)**: Manages deployment automation, infrastructure, and monitoring
- **[QA Lead](octoacme-roles-and-personas.md#qa-lead)**: Ensures quality gates are met before release
- **[Developers](octoacme-roles-and-personas.md#developers)**: Prepare code, tests, and technical documentation
- **[Product Manager](octoacme-roles-and-personas.md#product-managers)**: Reviews release scope and validates business requirements

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release Requirements
Before any release proceeds, the following must be completed:
- **Developers**: All acceptance criteria met and PRs merged
- **DevOps Engineer**: Passing CI and security scans
- **Release Manager**: Release notes drafted and reviewed
- **Release Manager**: Rollback / mitigation plan documented
- **QA Lead**: Smoke tests prepared and validated
- **Product Manager**: Release scope and impacts reviewed

## Deployment Checklist
- [ ] **Release Manager**: Deployment window scheduled and communicated (if needed)
- [ ] **DevOps Engineer**: Backup or snapshot completed (if applicable)
- [ ] **DevOps Engineer**: Deploy to staging environment
- [ ] **QA Lead**: Run smoke tests on staging and validate results
- [ ] **Release Manager**: Obtain go/no-go approval from stakeholders
- [ ] **DevOps Engineer**: Deploy to production (automated pipeline preferred)
- [ ] **DevOps Engineer**: Run post-deploy verifications and monitoring checks
- [ ] **Release Manager**: Announce release to stakeholders and support teams

## Rollback & Incident Playbook
If a deployment fails or causes a critical issue:
- **Release Manager**: Trigger incident response and notify on-call teams
- **DevOps Engineer**: Initiate rollback to last known-good release if necessary
- **DevOps Engineer**: Monitor system recovery and validate rollback success
- **Developers & QA Lead**: Triage root cause and capture action items
- **Release Manager**: Communicate incident status and resolution to stakeholders
- **Project Manager**: Schedule post-incident blameless retrospective

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
