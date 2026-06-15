# OctoAcme Project Management Docs

This README centralizes the OctoAcme project management process documents and provides a summary of our processes to help onboarding, discovery, and maintenance.

## Project Management Processes Overview

OctoAcme operates a structured, lifecycle-based project management approach grounded in customer value delivery and iterative execution. The framework spans five core phases: **Initiation** (validating business need and stakeholder alignment through a lightweight One-pager), **Planning** (breaking work into shippable increments with clear acceptance criteria and risk identification), **Execution** (managing day-to-day delivery through daily standups and sprint cycles), **Release** (standardizing deployment with pre-release checklists and rollback procedures), and **Close & Retrospective** (capturing learnings to drive continuous improvement).

The organizational model defines clear ownership through four primary personas: **Project Managers** coordinate schedules, risks, and communications; **Product Managers** own the vision and prioritize the backlog; **Developers** implement features and maintain quality through testing and code reviews; **QA/Testing** teams validate acceptance criteria and quality standards. Communication occurs through a structured cadence—daily standups (15 minutes), weekly delivery syncs, and monthly stakeholder updates—with a three-level escalation path for risks.

Quality and execution rigor are embedded throughout: Pull Request workflows with automated CI/CD, mandatory code reviews, unit and integration tests, and security scanning. Deployments follow pre-release checklists covering acceptance criteria, passing CI, and documented rollback plans. After each sprint or release, structured retrospectives capture learnings and generate prioritized action items, reinforcing a culture of continuous improvement.

## Links to Process Documents

- [Project Management Overview](octoacme-project-management-overview.md) — concise intro, principles, roles, and lifecycle.
- [Project Initiation Guide](octoacme-project-initiation.md) — one-pager template, initiation checklist, decision gate.
- [Project Planning](octoacme-project-planning.md) — backlog templates, planning activities, risk and dependency management.
- [Execution & Tracking](octoacme-execution-and-tracking.md) — team rhythm, PR workflow, QA, blocker escalation.
- [Risk Management & Communication](octoacme-risks-and-communication.md) — risk register, communication templates, escalation paths.
- [Release & Deployment Guide](octoacme-release-and-deployment.md) — deployment checklist, rollback playbook, release notes template.
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) — retrospective structure and action tracking.
- [Roles & Personas](octoacme-roles-and-personas.md) — role summaries and responsibilities used across docs.

## How to Use These Docs

- Update this README when adding or moving process docs.
- Link to these docs from new project repositories and from project one-pagers.
- Keep process docs in `docs/` and add process-specific working files to `.copilot/` when using Copilot Spaces.
- Use the [Process Doc Update issue template](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) to propose updates to any process document.

## Suggested Next Steps

- Add a link to this README from the repository root README.
- Reference these docs in new project charters and team onboarding materials.
