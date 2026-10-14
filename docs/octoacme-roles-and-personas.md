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

## Additional Operational & Cross-functional Personas (Proposed Additions)

The following personas are recommended additions. Each entry includes a short responsibility list and how the persona interacts with PM/PdM/Developers/QA and other roles.

---

### Delivery Lead / Technical Program Manager (TPM)

Role Summary
- Coordinates complex technical delivery across multiple teams, owns delivery cadence and cross-team dependencies.

Responsibilities
- Maintain and drive the delivery plan and milestone timelines
- Track cross-team dependencies and risk items; follow up until resolved
- Run cross-functional cadence meetings (dependency triage, integration checks)
- Ensure scope trade-offs are documented and communicated
- Escalate delivery blockers to PM/Engineering leadership as needed

Interactions
- PM: align on schedule, stakeholder communications, and resourcing constraints
- PdM: balance scope vs. timeline; clarify priority trade-offs
- Engineering Managers & Developers: secure capacity and unblock technical dependencies
- QA/SRE/Release Manager: coordinate integration testing and release readiness

---

### Release Manager

Role Summary
- Plans and coordinates releases, including runbooks, deployment windows, rollback procedures, and release communications.

Responsibilities
- Maintain release calendar and coordinate with stakeholders for windows
- Validate release readiness: PRs merged, CI green, smoke tests passing, and rollback plan documented
- Prepare release notes and communication templates
- Coordinate deployment steps and post-deploy verification
- Own rollback decision criteria and actions if needed

Interactions
- PM/PdM: agree release scope and timing
- SRE/Developers/QA: confirm operational readiness, runbooks, and monitoring
- Customer Success/Support: prepare customer-facing communications

---

### Site Reliability Engineer (SRE) / Observability Engineer

Role Summary
- Ensures system reliability in production; defines SLOs, monitoring, and incident runbooks.

Responsibilities
- Define and maintain SLOs, alerts, and dashboards
- Implement remediation/runbooks for common incidents
- Participate in on-call rotations and incident response
- Collaborate on capacity planning and performance testing
- Review and advise on production-impacting changes

Interactions
- Developers: advise on production fixes and design for reliability
- PM/PdM: inform trade-offs relating to reliability and operational cost
- Release Manager: validate monitoring and rollback readiness before release

---

### Security Champion / Security Liaison

Role Summary
- Advocates for security in product design and delivery; coordinates security scans and mitigations.

Responsibilities
- Perform threat modeling and security reviews during design and planning
- Coordinate static/dynamic analysis and vulnerability scans
- Raise and track security findings; recommend mitigations
- Liaise with central Security team for escalations and approvals

Interactions
- Developers: work closely during design reviews and remediation
- PM/PdM: communicate potential delivery impacts due to security fixes or mitigations
- Compliance/Privacy Lead: coordinate on regulatory or privacy-related security requirements

---

### UX Researcher / Designer

Role Summary
- Validates user needs, designs user flows and interfaces, and provides research insights for product decisions.

Responsibilities
- Conduct user research and usability testing
- Produce design assets, interaction patterns, and accessibility guidance
- Collaborate on acceptance criteria that reflect user outcomes
- Help prioritize features based on user impact

Interactions
- PdM: present research findings and recommend prioritization
- Developers: hand off designs and clarify behavior/edge-cases
- QA: ensure UX and accessibility acceptance criteria are testable

---

### Data Analyst / Analytics Engineer

Role Summary
- Defines success metrics, implements instrumentation, and validates outcomes against objectives.

Responsibilities
- Define event schemas and metrics needed for success criteria
- Work with engineering to implement instrumentation and dashboards
- Validate experiments and release impact through data analysis
- Provide metric-based recommendations for product decisions

Interactions
- PdM: agree on measurable success criteria and dashboard views
- Developers: implement tracking and ensure data quality
- PM: surface metric-driven risks or blockers impacting release

---

### QA Lead / Test Architect

Role Summary
- Owns test strategy, ensures critical test coverage, and coordinates test execution for releases.

Responsibilities
- Define overall testing strategy (automation vs manual, regression scopes)
- Maintain critical test suites and review test coverage gaps
- Coordinate manual exploratory testing and UAT where needed
- Sign off on release test readiness per agreed criteria

Interactions
- Developers: collaborate on testability and automation of critical flows
- Release Manager & PM: provide go/no-go recommendations based on test results
- SRE: coordinate production smoke tests and rollback test plans

---

### Customer Success Liaison / Support Representative

Role Summary
- Brings customer feedback to the product team and helps coordinate post-release communications and support escalations.

Responsibilities
- Provide prioritized customer feedback and usage patterns
- Coordinate release notes and customer-facing communications
- Triage production issues and coordinate with engineering/support during incidents
- Help prioritize critical bugs based on customer impact

Interactions
- PM/PdM: input for prioritization and success criteria
- Release Manager: collaborate on customer announcements
- Developers/QA: provide customer reproduction steps for issues

---

### Compliance / Privacy Lead (if applicable)

Role Summary
- Ensures project activities meet regulatory, privacy, and compliance obligations.

Responsibilities
- Check design and implementation against regulatory requirements
- Coordinate documentation and evidence for audits
- Recommend mitigations to meet compliance controls
- Sign off on releases that require compliance validation

Interactions
- PM: include compliance checkpoints in planning and release checklists
- PdM: align on scope or feature changes that affect compliance posture
- Security/Developers: coordinate required technical controls

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For each persona added, include:
  - A short Role Summary
  - 4–6 bullet Responsibilities
  - 2–3 explicit Interaction bullets describing handoffs with PM/PdM/Developers/QA (or other relevant roles)
- Consider adding a one-page "Release Readiness RACI" and a simple "Handoff matrix" showing who is Responsible/Accountable/Consulted/Informed for common activities (e.g., release decision, incident triage, compliance sign-off).

