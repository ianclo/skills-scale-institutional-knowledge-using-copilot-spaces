# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX Designer

### Role Summary
UX Designers are responsible for the end-to-end user experience of the product. They create wireframes, prototypes, and design specifications that ensure features are intuitive, accessible, and aligned with user needs.

### Responsibilities
- Research and validate user needs through interviews, usability tests, and analytics
- Create wireframes, prototypes, and high-fidelity design assets
- Define and document user flows, interaction patterns, and accessibility requirements
- Collaborate with Product Manager on feature requirements and acceptance criteria
- Work with Developers to ensure designs are implemented accurately
- Participate in sprint planning, reviews, and demos to provide design input and feedback

### Goals
- Deliver intuitive and accessible experiences that meet user needs
- Reduce re-work by resolving design ambiguity before development begins
- Advocate for the user in product and technical trade-off discussions

### Typical Communication
- Design reviews and critiques with PdM and Developers
- Usability test reports shared with PM and PdM
- Design specifications and assets in shared design tools (e.g., Figma)
- Participation in sprint planning and retrospectives

### Interactions with Existing Roles
- **Project Manager (PM):** Aligns on design milestones and timeline; surfaces design risks that may affect delivery dates.
- **Product Manager (PdM):** Collaborates closely on user requirements, success metrics, and acceptance criteria; validates that designs meet the product vision.
- **Developers:** Provides design specs, answers implementation questions, and reviews UI in-progress builds to catch deviations early.

---

## Release Manager

### Role Summary
Release Managers plan, coordinate, and oversee the safe delivery of software releases to production. They act as the hub between development, QA, and operations to ensure every release follows a repeatable, low-risk process.

### Responsibilities
- Create and maintain release plans, deployment windows, and communication schedules
- Coordinate go/no-go decisions with PM, PdM, and engineering leads
- Ensure rollback and mitigation plans are documented and rehearsed
- Manage staging deployments and smoke-test sign-off before production pushes
- Communicate release status, changes, and post-deploy results to stakeholders and support teams
- Track and resolve release blockers; escalate when needed

### Goals
- Deliver releases on schedule with minimal disruption to production
- Ensure rollback readiness so incidents can be contained quickly
- Maintain a clear audit trail of every release decision and deployment step

### Typical Communication
- Release readiness reports shared with PM and engineering leads
- Go/no-go meeting agendas and decision records
- Post-deploy summaries distributed to stakeholders and Support Lead
- Incident alerts and rollback notifications to the delivery team

### Interactions with Existing Roles
- **Project Manager (PM):** Syncs on release timelines and milestone gates; escalates blockers that threaten the release schedule.
- **Product Manager (PdM):** Confirms feature completeness and acceptance criteria are met before go/no-go sign-off.
- **Developers:** Coordinates deployment steps, environment readiness, and post-deploy verification tasks.

---

## Support Lead

### Role Summary
Support Leads represent the voice of the customer within the delivery team. They monitor customer-reported issues, synthesize support channel feedback, and ensure that product and engineering teams have visibility into real-world user impact.

### Responsibilities
- Monitor support queues, forums, and customer feedback channels
- Triage incoming issues and escalate bugs or recurring patterns to PM and PdM
- Maintain a feedback log that informs the product backlog and prioritization
- Coordinate with the Release Manager on post-release monitoring and hotfix needs
- Prepare support teams with release notes, FAQs, and known-issues documentation
- Participate in retrospectives to share customer experience insights

### Goals
- Minimize the customer impact of bugs, regressions, and unclear product behavior
- Ensure support teams are informed and prepared before each release
- Translate customer pain points into actionable product and process improvements

### Typical Communication
- Weekly support-trend summaries to PM and PdM
- Escalation alerts for critical or recurring customer issues
- Pre-release readiness notes and post-release incident updates
- Feedback reports feeding into retrospectives and backlog grooming

### Interactions with Existing Roles
- **Project Manager (PM):** Provides ongoing visibility into support volume and escalations; helps PM prioritize hotfix work.
- **Product Manager (PdM):** Shares customer feedback and usage patterns to inform roadmap decisions and acceptance criteria.
- **Developers:** Reports reproducible bugs with supporting evidence; validates fixes in staging before production rollout.

---

## Data Analyst

### Role Summary
Data Analysts define, track, and interpret the metrics that measure project and product success. They translate business objectives into measurable signals and provide data-driven insights that guide prioritization and decision-making across the team.

### Responsibilities
- Define KPIs and instrumentation requirements in collaboration with PdM and PM
- Build and maintain dashboards, reports, and automated alerts for project health and product usage
- Perform ad-hoc analysis to answer specific business or product questions
- Validate that metrics and tracking are implemented correctly during development
- Present findings in sprint reviews, stakeholder updates, and retrospectives
- Identify anomalies, trends, and opportunities for improvement based on data

### Goals
- Provide timely, accurate, and actionable data to support team decisions
- Ensure every significant initiative has clear, measurable success criteria and is tracked from day one
- Reduce reliance on assumptions by grounding product and project discussions in evidence

### Typical Communication
- Dashboard links and annotated reports shared with PM, PdM, and stakeholders
- Data requirements and tracking specifications for Developers
- Insight summaries at sprint demos and retrospectives
- Alerts and anomaly reports when metrics breach defined thresholds

### Interactions with Existing Roles
- **Project Manager (PM):** Provides project-level metrics (velocity, burndown, risk signals) and supports status reporting.
- **Product Manager (PdM):** Collaborates on defining success metrics and interpreting outcome data against product goals.
- **Developers:** Specifies instrumentation and event tracking requirements; validates data accuracy in development and staging.

---

## Subject Matter Expert (SME)

### Role Summary
Subject Matter Experts provide deep domain, technical, or industry knowledge that the core delivery team may not possess. They serve as trusted advisors during discovery, design, and review stages to ensure solutions are accurate, compliant, and aligned with real-world constraints.

### Responsibilities
- Provide domain or technical expertise when scoping, designing, or reviewing work
- Review deliverables (designs, specs, code, content) for accuracy, compliance, and best practices
- Answer ad-hoc questions from PM, PdM, and Developers during critical milestones
- Flag risks or misalignments between proposed solutions and domain standards
- Participate in key planning sessions, design reviews, or acceptance reviews as needed
- Help document domain knowledge in shared references for future team members

### Goals
- Prevent costly errors caused by domain knowledge gaps
- Improve the accuracy, quality, and credibility of project deliverables
- Ensure institutional knowledge is captured and shared rather than siloed

### Typical Communication
- Consultation sessions and written review feedback during design and planning
- Domain guidance documents or annotated specifications shared with the delivery team
- Attendance at key milestone reviews (scope definition, design review, acceptance sign-off)
- Availability via async channels (chat, comments) for quick expert queries

### Interactions with Existing Roles
- **Project Manager (PM):** Advises on domain-specific risks and constraints that may affect schedule or scope; available for escalation on complex decisions.
- **Product Manager (PdM):** Validates that product decisions align with domain requirements, regulatory standards, or customer expectations.
- **Developers:** Reviews technical designs and implementation approaches for domain correctness; provides reference materials and answers targeted implementation questions.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

