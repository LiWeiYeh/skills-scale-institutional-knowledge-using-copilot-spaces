# OctoAcme Project Management Docs

This README centralizes OctoAcme's project management process documents and provides a short summary of the operating model used across the organization. It is intended to be the primary entry point for onboarding, process discovery, and linking this guidance into project repositories or Copilot Spaces context.

## Brief summary of the project management processes used by OctoAcme

OctoAcme runs projects through a staged lifecycle that begins with initiation and ends with retrospective and continuous improvement. During initiation, teams validate the business need, identify stakeholders, and capture a Project One-pager with goals, metrics, risks, and a high-level timeline. Planning then turns the approved initiative into a backlog with acceptance criteria, estimates, dependencies, milestones, and a Definition of Done. During execution, work is tracked through a project board with clear workflow stages, daily standups, review demos, and defined escalation paths when blockers arise.

The organization also emphasizes clear ownership and communication. Product and project leads define outcomes and priorities, developers and QA deliver and validate work, and stakeholders provide alignment, approvals, and feedback. Weekly status updates, milestone reviews, and standard incident communication templates keep work visible and decision-making consistent across teams. Risk management and release governance are embedded in the process as well, with a risk register, escalating dependencies, and documented rollback plans.

Quality is preserved through a disciplined delivery model that includes unit, integration, and end-to-end smoke testing as appropriate, along with CI checks, security scanning, and manual QA for critical features. In release and deployment, teams complete pre-release validation, verify smoke tests in staging, and only then deploy to production with post-deploy checks and stakeholder notifications. After each sprint, release, or significant incident, the team runs retrospectives to capture lessons learned, assign action items, and improve the process over time.

## Docs and links

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospectives & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## How to use these docs

- Use this README as the hub for process guidance and onboarding.
- Link it from project repositories or internal documentation when creating new work.
- Keep the links and summaries updated as documents evolve.
- Add this folder to Copilot Spaces context when you want project guidance surfaced during planning and execution.

## Quick process overview

- Initiation: Validate need, define stakeholders, and decide whether to move forward.
- Planning: Build backlog, estimate scope, and agree on milestones and Definition of Done.
- Execution & Tracking: Run standups, manage PRs and CI, and escalate blockers as needed.
- Release & Deployment: Complete checks, test in staging, deploy with rollback readiness.
- Risk Management & Communication: Maintain status visibility and escalate appropriately.
- Retrospectives & Continuous Improvement: Capture actions, owners, and improvements.
- Roles & Personas: Clarify responsibilities across PM, Product, Engineering, QA, and stakeholders.
