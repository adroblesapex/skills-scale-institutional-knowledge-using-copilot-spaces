# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Core Personas

### Developers

#### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

#### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

#### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

#### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

### Product Managers

#### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

#### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

#### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

#### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

### Project Managers

#### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

#### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

#### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

#### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Additional Personas

These personas represent cross-cutting and specialty roles that commonly influence delivery, risk, and quality. Include these roles as needed for your projects.

### Release Manager

#### Role Summary
Release Managers coordinate releases across environments, manage deployment windows, and ensure rollback and mitigation plans are in place. They own the release process and serve as the single point of accountability for moving code to production safely.

#### Responsibilities
- Schedule and coordinate deployments with CI/CD and operations teams
- Own release checklists and pre-release verification steps
- Perform post-deployment verifications and smoke tests
- Communicate release status and timeline to stakeholders
- Document and execute rollback procedures when needed
- Track and report on release metrics (success rate, rollback frequency, deployment time)

#### When to Involve
- During planning phase: to define release windows and dependencies
- Pre-release: to coordinate final testing and deployment readiness
- Deployment: to execute and verify the release
- Post-incident: to run retrospective and update runbooks

#### Interaction with Existing Roles
- **PM**: Coordinates release timing and stakeholder notifications
- **Developers**: Works with them on deployment readiness and rollback testing
- **QA**: Ensures release verification steps are complete before go-live
- **Support Liaison**: Ensures support teams are ready for customer impact

---

### Security Champion

#### Role Summary
Security Champions own security considerations within the delivery team and coordinate with the security organization. They ensure secure design practices are followed, security reviews occur, and vulnerabilities are remediated promptly.

#### Responsibilities
- Perform threat modeling for new features during design phase
- Ensure required security scans and remediation are tracked in the risk register
- Advise on secure design patterns and review PRs for security concerns
- Coordinate security testing (SAST, DAST, dependency scanning) with CI/CD
- Escalate critical security findings and coordinate remediation timelines
- Conduct security awareness sessions for the project team

#### When to Involve
- Planning: to identify security requirements and threat models
- Development: to review design and code for security concerns
- Pre-release: to ensure security scans pass and vulnerabilities are resolved
- Incidents: to triage and respond to security-related issues

#### Interaction with Existing Roles
- **Developers**: Partners on secure coding practices and PR reviews
- **PM**: Flags security risks that impact timelines or scope
- **QA**: Coordinates security testing and acceptance criteria
- **Release Manager**: Ensures security gates are passed before deployment

---

### UX Researcher / Designer

#### Role Summary
UX Researchers and Designers validate user needs, ensure designs meet usability and accessibility requirements, and gather evidence that the product solves customer problems effectively.

#### Responsibilities
- Run lightweight research and usability testing with users
- Produce design assets, wireframes, and accessibility checks
- Define user-acceptance criteria related to UX and accessibility
- Partner on design reviews and iterate based on feedback
- Document design decisions and rationale for future reference
- Ensure accessibility standards (WCAG) are met and tested

#### When to Involve
- Initiation: to validate problem statement and user needs
- Planning: to define UX acceptance criteria and design requirements
- Development: to clarify implementation details and answer design questions
- QA/Acceptance: to validate UX meets acceptance criteria before release

#### Interaction with Existing Roles
- **Product Manager**: Translates outcomes and user insights into features
- **Developers**: Clarifies implementation details and feasibility of designs
- **QA**: Works together on usability and accessibility acceptance tests
- **Support Liaison**: Gathers user feedback to inform future iterations

---

### Data Analyst

#### Role Summary
Data Analysts define measurement plans, instrument success metrics, and validate that projects are achieving intended outcomes. They provide data-driven insights to support decision-making throughout the project lifecycle.

#### Responsibilities
- Propose and define metrics to validate project outcomes
- Instrument code and dashboards to collect and visualize key metrics
- Run analyses to inform go/no-go decisions for releases
- Help define success criteria for experiments and feature flags
- Provide regular reporting on metric trends and business impact
- Identify anomalies and investigate root causes

#### When to Involve
- Initiation: to define success metrics in the project one-pager
- Planning: to establish baseline metrics and monitoring approach
- Execution: to track progress toward success metrics
- Release: to validate impact and support decision to rollout or rollback
- Retrospective: to measure final impact and inform lessons learned

#### Interaction with Existing Roles
- **Product Manager**: Partners on success metrics and impact measurement
- **Project Manager**: Supports status reporting and decision-making
- **Developers**: Ensures instrumentation requirements are built into features
- **QA**: Works together on test data and validation approaches

---

### Support Liaison

#### Role Summary
Support Liaisons bridge product delivery and customer-facing support teams. They provide customer-impact insight, help teams understand support burden, and ensure support and customer success teams are prepared for new features.

#### Responsibilities
- Provide customer-impact insight and triage recurring support issues
- Help craft support runbooks, FAQs, and customer-facing documentation
- Surface escalation-worthy incidents and customer feedback to PM and engineering
- Represent support perspective during planning and design reviews
- Coordinate training and readiness for support teams before release
- Track customer satisfaction and support metrics related to new features

#### When to Involve
- Planning: to represent customer support perspective and constraints
- Development: to provide customer context and inform design decisions
- Pre-release: to prepare support team and documentation
- Post-release: to monitor support volume and customer feedback
- Incidents: to escalate critical customer-impacting issues

#### Interaction with Existing Roles
- **Product Manager**: Surfaces customer feedback and support trends
- **Project Manager**: Escalates critical incidents and customer impact
- **Developers**: Partners on design decisions that affect support burden
- **Release Manager**: Coordinates support team readiness and communications

---

### QA Automation Lead

#### Role Summary
QA Automation Leads own the test automation strategy and CI/CD test coverage for projects. They ensure quality gates are in place, tests are maintainable, and the team has confidence in automated verification.

#### Responsibilities
- Maintain test suites and ensure CI integration for all acceptance criteria
- Improve flaky-test mitigation and failure reporting
- Coach developers on testability and acceptance criteria
- Define test strategy and approach for the project
- Identify and remediate gaps in test coverage
- Own smoke tests and critical-path testing for releases

#### When to Involve
- Planning: to define test strategy and acceptance criteria
- Development: to coach developers and review test coverage
- Code review: to assess testability and test quality of PRs
- Pre-release: to ensure test gates are passing and critical paths are covered
- Post-incident: to identify test gaps that should have caught the issue

#### Interaction with Existing Roles
- **Developers**: Coaches on testability, test quality, and acceptance criteria
- **Project Manager**: Reports on test coverage and quality metrics
- **Release Manager**: Ensures test gates pass before deployment approval
- **QA/Testing**: Partners on comprehensive test coverage and automation

---

## How These Personas Are Used

- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance
- When staffing a project, map team members to these personas to clarify roles and responsibilities
- Use the "When to Involve" guidance to determine which personas should participate in each phase
- Not every project will need all personas—scale to fit your organization and project complexity
