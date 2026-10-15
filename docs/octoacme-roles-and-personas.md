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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Suggested Personas (proposed additions)

Note: these personas are recommended additions to clarify ownership for operational and cross-cutting concerns. For each persona below we include a short role summary, responsibilities, interactions with existing roles, when to involve, and a concise escalation path.

### Technical Program Manager (TPM)

Role Summary
- TPMs coordinate cross-team technical dependencies and program-level technical planning to ensure complex integrations and architectural decisions progress smoothly.

Responsibilities
- Coordinate cross-team technical dependencies and integration plans
- Maintain program-level schedule for multi-team initiatives
- Run technical risk assessments and surface mitigation options
- Facilitate architecture trade-off discussions and decision tracking

Interaction
- Works with Project Manager for schedule alignment and risk communication
- Engages Engineering Managers and Developers to unblock integration issues
- Partners with Product Manager (PdM) to align scope with technical constraints

When to involve
- Planning for multi-team features, design/architecture reviews, and pre-release integration checks

Escalation path
- Escalate unresolved technical dependency risks to Engineering leadership and Product Lead

---

### Delivery Lead

Role Summary
- The Delivery Lead drives day-to-day execution for a release or milestone, ensuring readiness and completion of delivery checklists.

Responsibilities
- Own sprint readiness and ensure backlog items are shippable
- Track completion of release and deployment checklists
- Coordinate release communications and run pre-release readiness reviews
- Monitor release gates and acceptance criteria

Interaction
- Coordinates status and risks with the Project Manager
- Works with Release Manager on deploy windows and runbooks
- Partners with QA to ensure acceptance gating

When to involve
- Sprint planning, release readiness reviews, and during release execution

Escalation path
- Escalate delivery blockers to the Project Manager and Product Lead

---

### Release Manager

Role Summary
- The Release Manager owns release orchestration, deployment runbooks, and rollback/mitigation procedures to minimize production risk.

Responsibilities
- Maintain the release plan and deployment runbook
- Coordinate CI/CD pipelines and approve production deploys
- Validate rollback procedures and trigger rollbacks when necessary
- Coordinate post-deployment verification steps

Interaction
- Works with Delivery Lead to confirm readiness and deploy windows
- Collaborates with Observability/Platform Engineers for post-deploy checks
- Notifies Support Liaison and stakeholders of release timing and potential impacts

When to involve
- Release planning, cutover windows, and production deploys

Escalation path
- Escalate deployment failures to on-call teams and Project Manager; escalate critical incidents to Sponsor/Leadership

---

### Observability / Platform Engineer

Role Summary
- Observability/Platform Engineers ensure adequate monitoring, alerting, and dashboards are in place to verify feature health and support incident triage.

Responsibilities
- Define monitoring and alerting requirements for new features
- Build and maintain dashboards and runbooks for observability
- Support post-deploy verification and incident triage
- Advise on instrumentation and telemetry best practices

Interaction
- Partners with Developers for instrumentation implementation
- Shares metrics and dashboards with Product Manager and Data Analyst
- Works with Support Liaison during incidents to interpret alerts

When to involve
- During design for instrumentation, pre-release verification, and incident response

Escalation path
- Escalate persistent observability gaps to Platform or Engineering leadership

---

### Security Representative (Security On-call)

Role Summary
- Security Representatives review security implications of features and support security incident response to reduce vulnerabilities and maintain compliance.

Responsibilities
- Review security impact and approve deviations or exceptions
- Participate in threat modeling for high-risk changes
- Support security incident response and remediation
- Maintain and communicate security best practices

Interaction
- Engages during planning, design reviews, and code review as needed
- Coordinates with Developers and Engineering leadership on fixes
- Escalates critical security issues to Security leadership

When to involve
- For features affecting sensitive data, external integrations, or when security review is required; involved in post-incident response

Escalation path
- Escalate to Security Leadership and Incident Response team for critical vulnerabilities

---

### UX Researcher / Designer Representative

Role Summary
- UX Researchers and Designers ensure user insights and usability criteria are captured and validated, improving product usability and acceptance.

Responsibilities
- Capture research insights and translate them into acceptance criteria
- Provide design guidance and accessibility reviews
- Run lightweight validation or usability tests as needed
- Ensure clarity of user-facing flows and acceptance criteria

Interaction
- Collaborates with Product Manager on user-facing decisions
- Works with Developers to resolve UI/UX implementation constraints
- Shares findings with Project Manager to inform priorities

When to involve
- During feature scoping, design reviews, and pre-release validation

Escalation path
- Escalate significant usability risks to Product Lead and Project Manager

---

### Support Liaison / Customer Success Representative

Role Summary
- The Support Liaison provides customer context, manages escalations during and after releases, and validates incident resolution from the customer perspective.

Responsibilities
- Provide customer impact context for incidents and releases
- Manage support escalations and coordinate communications with customers
- Validate fixes from a customer-experience perspective
- Maintain knowledge transfer between engineering and support teams

Interaction
- Works with Project Manager and Release Manager for release communications
- Partners with Observability Engineers to prioritize alerts and dashboards
- Collaborates with Developers to reproduce and validate issues

When to involve
- Pre-release communications, during incidents, and in post-incident customer updates

Escalation path
- Escalate major customer-impacting issues to Product Lead and Sponsor

---

### Data Analyst

Role Summary
- Data Analysts define and measure success metrics, set up dashboards, and perform post-release analysis to inform product decisions.

Responsibilities
- Define success metrics and measurement plans
- Create dashboards and reports to track feature impact
- Perform post-release analyses and surface insights
- Support instrumentation validation and A/B analysis

Interaction
- Partners with Product Manager on success criteria and metric definitions
- Works with Developers and Observability Engineers to ensure proper instrumentation
- Shares analysis with Project Manager and stakeholders to inform next steps

When to involve
- During planning to define success metrics, and post-release for impact analysis

Escalation path
- Escalate measurement gaps or critical data issues to Product Lead and Engineering leadership

---

For each persona above, consider adding a one-line "When to involve" note and a single-line "Escalation path" (already included). These additions are intended to be concise to enable quick review and iteration with stakeholders.
