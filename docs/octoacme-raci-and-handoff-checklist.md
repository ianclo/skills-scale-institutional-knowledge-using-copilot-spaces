# OctoAcme — RACI Responsibility Map & Cross-functional Handoff Checklist

This document maps responsibilities across the full project lifecycle and provides practical handoff checklists for the transitions between Planning → Execution → Release → Support.

For full persona descriptions, see [Roles & Personas](./octoacme-roles-and-personas.md).

**RACI key:** R = Responsible | A = Accountable | C = Consulted | I = Informed

---

## RACI Responsibility Map

### Initiation

| Activity | PM | PdM | Dev | UX Designer | Release Mgr | Support Lead | Data Analyst | SME |
|----------|----|-----|-----|-------------|-------------|--------------|--------------|-----|
| Draft project one-pager | R | A | I | C | I | I | C | C |
| Define success metrics | C | A | I | C | I | I | R | C |
| Stakeholder alignment | R | A | I | I | I | C | I | C |
| Go/no-go decision for planning | A | A | C | C | I | I | C | C |

### Planning

| Activity | PM | PdM | Dev | UX Designer | Release Mgr | Support Lead | Data Analyst | SME |
|----------|----|-----|-----|-------------|-------------|--------------|--------------|-----|
| Backlog creation and prioritization | C | A | C | C | I | C | C | C |
| Define acceptance criteria | C | A | R | R | I | C | C | C |
| Design wireframes / user flows | I | C | C | A/R | I | I | I | C |
| KPI and tracking instrumentation | C | A | C | C | I | I | R | C |
| Release plan and milestone map | A | C | C | C | R | C | I | I |
| Define Definition of Done | A | C | R | C | C | I | C | I |
| Risk register setup | R | C | C | C | C | C | I | C |
| SME review of scope / requirements | C | A | C | C | I | I | I | R |

### Execution

| Activity | PM | PdM | Dev | UX Designer | Release Mgr | Support Lead | Data Analyst | SME |
|----------|----|-----|-----|-------------|-------------|--------------|--------------|-----|
| Feature development | I | C | R/A | C | I | I | I | C |
| UI implementation review | I | C | R | A | I | I | I | I |
| Metrics / analytics instrumentation | I | C | R | I | I | I | A | I |
| Daily standup facilitation | R | I | R | C | I | I | I | I |
| Sprint demo / review | R | A | R | R | I | C | R | C |
| Risk register updates | R | C | C | I | C | C | I | I |
| Blocker escalation | A | C | R | C | C | C | I | C |
| Domain / compliance review | C | A | C | C | I | I | I | R |

### Release

| Activity | PM | PdM | Dev | UX Designer | Release Mgr | Support Lead | Data Analyst | SME |
|----------|----|-----|-----|-------------|-------------|--------------|--------------|-----|
| Release readiness report | C | C | C | C | R/A | I | I | I |
| Go/no-go sign-off | A | A | C | C | R | C | C | I |
| Deployment execution | I | I | R | I | A | I | I | I |
| Post-deploy verification | C | C | R | I | A | C | C | I |
| Release notes and announcements | C | C | I | I | R | A | I | I |
| Support team briefing | I | I | I | I | C | R/A | I | I |
| Post-release metrics check | I | C | I | I | I | C | R/A | I |
| Rollback decision | A | C | R | I | R | C | I | I |

### Retrospective & Continuous Improvement

| Activity | PM | PdM | Dev | UX Designer | Release Mgr | Support Lead | Data Analyst | SME |
|----------|----|-----|-----|-------------|-------------|--------------|--------------|-----|
| Retrospective facilitation | R/A | C | R | C | C | C | C | I |
| Customer feedback summary | I | C | I | I | I | R/A | C | I |
| Metrics / outcome review | C | A | I | C | I | C | R | I |
| Action item ownership assignment | A | C | C | C | C | C | C | I |

---

## Cross-functional Handoff Checklists

### Planning → Execution Handoff

Use this checklist before the delivery team begins building to confirm that planning outputs are complete and ownership is clear.

**PM confirms:**
- [ ] Project one-pager approved and available in the project repo
- [ ] Backlog is prioritized, estimated, and has clear acceptance criteria
- [ ] Definition of Done is documented and agreed by the team
- [ ] Risk register initialized with known risks and owners
- [ ] Release plan and milestone dates agreed with Release Manager

**PdM confirms:**
- [ ] Feature requirements and acceptance criteria are finalized
- [ ] Success metrics and KPIs are defined and shared with Data Analyst
- [ ] SME review completed for any domain-specific requirements

**UX Designer confirms:**
- [ ] Wireframes / prototypes available and reviewed for all in-scope user flows
- [ ] Design assets and specs accessible to Developers
- [ ] Accessibility requirements documented in acceptance criteria

**Data Analyst confirms:**
- [ ] KPIs and instrumentation requirements documented
- [ ] Tracking plan shared with Developers for implementation

**Release Manager confirms:**
- [ ] Release window identified and communicated to stakeholders
- [ ] Rollback plan drafted (even if rough at this stage)

---

### Execution → Release Handoff

Use this checklist before initiating the release process to confirm readiness.

**PM confirms:**
- [ ] All planned backlog items are Done (per Definition of Done)
- [ ] Risk register reviewed and no open blockers
- [ ] Stakeholder notification drafted or scheduled

**PdM confirms:**
- [ ] Acceptance criteria verified for each shipped feature
- [ ] Release notes reviewed and approved

**Developers confirm:**
- [ ] All CI checks passing (tests, lint, security scans)
- [ ] Code merged to release branch
- [ ] Post-deploy verification steps documented

**UX Designer confirms:**
- [ ] UI implementation reviewed against design specs
- [ ] Critical usability issues resolved or explicitly deferred

**Data Analyst confirms:**
- [ ] All tracking and instrumentation is live and validated in staging
- [ ] Dashboards and alerts configured for post-release monitoring

**Release Manager confirms:**
- [ ] Go/no-go meeting scheduled
- [ ] Deployment runbook complete and reviewed
- [ ] Rollback plan finalized and communicated to on-call team
- [ ] Support Lead briefed on changes and known issues

**Support Lead confirms:**
- [ ] Support team has received release notes and FAQs
- [ ] Customer-facing documentation is updated (if applicable)
- [ ] Post-release monitoring responsibilities are assigned

---

### Release → Support Handoff

Use this checklist after a successful deployment to transition from release mode to steady-state support.

**Release Manager confirms:**
- [ ] Post-deploy verification completed with no critical issues
- [ ] Release summary distributed to PM, PdM, and stakeholders
- [ ] Incident response bridge closed (if one was opened)

**Support Lead confirms:**
- [ ] Support team is monitoring for new customer reports
- [ ] Known issues list published in support knowledge base
- [ ] Escalation contacts for this release are documented

**Data Analyst confirms:**
- [ ] Post-release metrics are tracked and baseline established
- [ ] Alerts are active for key health indicators
- [ ] First metrics review scheduled (e.g., 1-week and 4-week post-release)

**PM confirms:**
- [ ] Retrospective scheduled
- [ ] Remaining follow-up items added to the project backlog

---

## Role Interaction Summary

The diagram below shows the primary collaboration lines between roles across the lifecycle.

```
Initiation / Planning
  PdM ──────► UX Designer   (requirements → design)
  PdM ──────► Data Analyst  (goals → KPIs)
  PdM ──────► SME           (requirements → domain review)
  PM  ──────► Release Mgr   (scope → release plan)

Execution
  PdM ──────► Developers    (acceptance criteria)
  UX Designer ─► Developers (design specs)
  Data Analyst ─► Developers (instrumentation specs)
  SME ──────► Developers    (domain guidance)
  PM  ──────► All           (status, risks, blockers)

Release
  Release Mgr ─► Developers (deployment coordination)
  Release Mgr ─► PM/PdM     (go/no-go)
  Release Mgr ─► Support Lead (release notes, briefing)

Post-Release / Support
  Support Lead ─► PM/PdM   (customer feedback, escalations)
  Data Analyst ─► PM/PdM   (metrics outcomes)
  PM ──────────► All       (retrospective, action items)
```
