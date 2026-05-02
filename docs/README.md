# OctoAcme Project Management — Docs Overview

This folder contains the process documentation for how OctoAcme manages cross-functional projects. The docs cover the full project lifecycle, key roles, communication practices, and quality standards. Use this README as an entry point to explore the detailed guides below.

## Overview

OctoAcme follows a lightweight, end-to-end project lifecycle: **Initiation → Planning → Execution → Release → Retrospective/Continuous Improvement**. Work begins with a [Project Initiation](./octoacme-project-initiation.md) phase where a one-pager or charter is created to clarify the problem, define SMART goals and success metrics, identify stakeholders, and establish an initial timeline and risk list. Once approved, the [Planning](./octoacme-project-planning.md) phase converts the initiative into an actionable backlog with prioritised items, clear acceptance criteria, a Definition of Done, mapped dependencies, and a milestone/release plan.

Roles are clearly defined to ensure ownership and cross-functional delivery. A named **Project Manager (PM)** coordinates schedules, execution, risks, and stakeholder communications; the **Product Manager (PdM)** defines outcomes, prioritises the backlog, and measures impact; **Developers** design and implement features with testability in mind; and **QA/Testing** validates quality and acceptance. Full persona details are available in the [Roles & Personas](./octoacme-roles-and-personas.md) guide. The team operates with iterative delivery, data-informed decisions, and psychological safety so that issues can be surfaced early and learning is continuous.

Execution and tracking are anchored in a consistent team rhythm and transparent workflow management. OctoAcme uses a project board (e.g., GitHub Projects) with standard columns (Backlog → Ready → In Progress → In Review → QA → Done) and a disciplined PR workflow: small PRs, issue links, CI checks before review, and at least one approval before merging. Progress is monitored via delivery metrics such as velocity and burndown, alongside operational dashboards for errors, latency, and usage. See the [Execution & Tracking](./octoacme-execution-and-tracking.md) guide for details.

Communication and risk management are treated as continuous practices. The team maintains a [Risk Register](./octoacme-risks-and-communication.md) (description, impact/likelihood, owner, mitigation, status) reviewed at weekly syncs, with a clear escalation path from team triage up to sponsor-level for business-impacting issues. [Releases](./octoacme-release-and-deployment.md) are standardised with pre-release requirements, a deployment checklist (staging → smoke tests → production → post-deploy verification), and an incident/rollback playbook. After each sprint, release, or milestone, [Retrospectives](./octoacme-retrospective-and-continuous-improvement.md) capture action items with owners and feed improvements back into the backlog.

## Docs in this folder

| File | Description |
|------|-------------|
| [octoacme-project-management-overview.md](./octoacme-project-management-overview.md) | High-level overview of OctoAcme's PM approach, principles, and lifecycle |
| [octoacme-project-initiation.md](./octoacme-project-initiation.md) | Initiation guide: one-pager template, stakeholder alignment, go/no-go |
| [octoacme-project-planning.md](./octoacme-project-planning.md) | Planning guide: backlog, estimation, Definition of Done, release plan |
| [octoacme-execution-and-tracking.md](./octoacme-execution-and-tracking.md) | Execution guide: team rhythm, PR workflow, quality, metrics, escalation |
| [octoacme-risks-and-communication.md](./octoacme-risks-and-communication.md) | Risk register, lifecycle, stakeholder communication templates |
| [octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md) | Persona definitions for PM, PdM, Developer, QA, and Stakeholder |
| [octoacme-release-and-deployment.md](./octoacme-release-and-deployment.md) | Release checklist, deployment steps, incident/rollback playbook |
| [octoacme-retrospective-and-continuous-improvement.md](./octoacme-retrospective-and-continuous-improvement.md) | Retrospective formats, cadence, and continuous improvement practices |
