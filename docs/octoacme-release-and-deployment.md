# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Roles & Ownership

| Activity | Owner | Participants |
|----------|-------|--------------|
| Release plan and schedule | **Release Manager** | PM, PdM, Developers |
| Go/no-go decision | PM + PdM | Release Manager, QA |
| Deployment execution | **Release Manager** + Developers | QA |
| Rollback decision | **Release Manager** | PM, on-call engineer |
| Post-release communication | **Release Manager** | Support Lead, PM |
| Support readiness (FAQs, release notes) | **Support Lead** | Release Manager |

See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions of the Release Manager and Support Lead roles.

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted by Release Manager
- Rollback / mitigation plan documented and reviewed
- Smoke tests prepared
- Support Lead briefed on changes and known issues

## Deployment Checklist
- [ ] Deployment window scheduled by Release Manager (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Go/no-go sign-off from PM and PdM
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (Release Manager)
- [ ] Support Lead confirms support team is ready

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Release Manager triggers incident response and notifies on-call
  - Rollback to last known-good release if necessary
  - Support Lead monitors customer impact and provides updates
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
