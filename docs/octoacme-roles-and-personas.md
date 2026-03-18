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

## QA / Testing

### Role Summary
QA/Testing contributors validate features and acceptance criteria during development. For quality strategy, test coverage ownership, and release gate authority, see the [QA Lead](#qa-lead) role below.

### Responsibilities
- Execute test cases and exploratory testing on in-progress features
- Report defects with clear reproduction steps
- Validate bug fixes before closing tickets
- Support the QA Lead in building and maintaining test suites

### Goals
- Catch regressions and defects before they reach end users
- Provide rapid feedback loops to developers during active sprints

### Typical Communication
- Daily standups and sprint demos
- Defect reports and test result summaries

---

## QA Lead

### Role Summary
The QA Lead owns the quality strategy, test coverage, and quality gates for the project. Distinct from individual QA/Testing contributors, the QA Lead is accountable for overall release readiness and defines standards that the entire team follows.

### Responsibilities
- Define and maintain the test strategy and quality standards
- Own the Definition of Done criteria related to quality
- Coordinate test coverage across unit, integration, and end-to-end layers
- Run and sign off quality gates before releases
- Triage defects, assign severity, and track resolution
- Collaborate with DevOps to integrate automated testing into CI/CD

### Goals
- Ensure releases meet quality and reliability standards before reaching production
- Shift quality left by embedding test thinking early in the development cycle
- Build a sustainable, automated test suite that reduces manual regression effort

### Typical Communication
- Sprint ceremonies and demo/review sessions
- Defect triage meetings with Developers and PM
- Pre-release readiness sign-off communications
- Test strategy and coverage reports to stakeholders

### Interactions with Existing Roles
- **Project Manager**: Reports quality status and flags risks that may block release windows.
- **Product Manager**: Aligns acceptance criteria with testable quality conditions.
- **Developers**: Reviews test coverage, pairs on hard-to-test areas, and reviews PRs for testability.
- **Release Manager**: Co-owns release readiness decision; must sign off before a release window opens.
- **DevOps / Platform Engineer**: Collaborates on CI/CD pipeline test stages and test environment stability.
- **Stakeholders**: Communicates release quality metrics and outstanding known issues.

---

## UX Designer

### Role Summary
The UX Designer is responsible for the user experience: research, interaction design, prototyping, and usability validation. They translate user needs and business goals into clear, testable designs.

### Responsibilities
- Conduct user research, interviews, and usability tests
- Create wireframes, flows, and high-fidelity prototypes
- Maintain a design system and component guidelines
- Collaborate on feature definitions to advocate for usability
- Participate in acceptance criteria reviews to ensure UX intent is captured

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce design-to-development rework through clear, validated specifications
- Keep a consistent design language across the product

### Typical Communication
- Design reviews with Product Manager, Developers, and stakeholders
- Usability test result summaries shared with the broader team
- Figma or equivalent design files linked from backlog items

### Interactions with Existing Roles
- **Project Manager**: Coordinates design timelines with project milestones to avoid last-minute redesigns.
- **Product Manager**: Partners to ensure designs align with product vision and success metrics.
- **Developers**: Handoffs via annotated design files; available for implementation Q&A during development.
- **QA Lead**: Reviews final builds against design specifications to catch visual and interaction regressions.
- **Stakeholders**: Presents prototypes and research findings for feedback and sign-off.

---

## Release Manager

### Role Summary
The Release Manager owns the release calendar, production deployment windows, and cross-functional release coordination. They ensure releases are planned, communicated, and executed safely.

### Responsibilities
- Maintain the release calendar and communicate windows to all stakeholders
- Coordinate go/no-go decisions with QA Lead, DevOps, and PM
- Own the release notes process, ensuring completeness before publish
- Drive rollback decisions during incidents related to recent releases
- Gate releases against pre-release requirements (CI, security scans, smoke tests)

### Goals
- Make releases predictable, low-risk events
- Reduce time-to-production for approved changes
- Maintain a clear release history for audit and support teams

### Typical Communication
- Release planning meetings and release calendar updates
- Go/no-go announcements to stakeholders and support teams
- Post-release summaries and incident retrospectives

### Interactions with Existing Roles
- **Project Manager**: Aligns release windows with project milestones and sprint cadences.
- **Product Manager**: Ensures release scope matches planned features and communicates changes to stakeholders.
- **QA Lead**: Requires quality gate sign-off before declaring a release ready.
- **DevOps / Platform Engineer**: Collaborates on deployment execution and rollback procedures.
- **Developers**: Confirms all PRs are merged and artifacts are ready before the release window.
- **Stakeholders**: Distributes release notes and coordinates stakeholder communication.

---

## DevOps / Platform Engineer

### Role Summary
The DevOps / Platform Engineer maintains the CI/CD pipelines, infrastructure, and developer tooling. They enable fast, reliable, and secure delivery by automating build, test, and deployment workflows.

### Responsibilities
- Build and maintain CI/CD pipelines for automated testing and deployment
- Manage infrastructure provisioning (cloud, containers, networking)
- Implement and monitor security scanning and compliance checks
- Support test environment stability and parity with production
- Respond to infrastructure incidents and improve reliability (SLOs)

### Goals
- Reduce mean time to deploy and mean time to recover
- Ensure infrastructure is secure, observable, and cost-efficient
- Enable developers to self-serve environment and tooling needs

### Typical Communication
- Infrastructure change announcements and maintenance windows
- Incident alerts and post-mortems
- CI/CD status updates during release windows

### Interactions with Existing Roles
- **Project Manager**: Communicates planned maintenance or infrastructure risks that may affect delivery timelines.
- **Developers**: Provides tooling, pipeline support, and guidance on cloud-native best practices.
- **QA Lead**: Maintains test environments and integrates automated test stages into pipelines.
- **Release Manager**: Executes deployment operations and supports rollback during releases.
- **Stakeholders**: Informs on infrastructure SLOs and availability commitments.

---

## Business Analyst

### Role Summary
The Business Analyst bridges stakeholders and the delivery team by gathering, refining, and tracing requirements. They ensure that user stories reflect real business needs and that nothing important is lost in translation.

### Responsibilities
- Facilitate requirements discovery workshops with stakeholders and product teams
- Document business rules, process flows, and functional requirements
- Write or review user stories and acceptance criteria for clarity
- Maintain requirements traceability across backlog and test cases
- Identify scope gaps and flag ambiguities early

### Goals
- Eliminate requirement ambiguity before development begins
- Ensure delivered solutions match stakeholder intent
- Create a shared understanding between technical and non-technical participants

### Typical Communication
- Requirements workshops and discovery meetings
- User story refinement sessions with PM and Developers
- Status updates to stakeholders on open questions and decisions

### Interactions with Existing Roles
- **Project Manager**: Feeds refined requirements into project scope and timeline estimates.
- **Product Manager**: Partners on backlog refinement and acceptance criteria quality.
- **Developers**: Answers clarifying questions during implementation and reviews technical interpretations of requirements.
- **UX Designer**: Aligns on user flows and validates that designs satisfy documented requirements.
- **QA Lead**: Provides requirement context to support test case design and traceability.
- **Stakeholders**: Primary liaison for gathering needs and communicating back decisions.

---

## Stakeholder Subtypes

OctoAcme projects involve several distinct stakeholder types, each with different communication expectations and levels of involvement.

### Internal Customer

#### Role Summary
An internal customer is a team or individual within OctoAcme who depends on the project's output to perform their own work (e.g., a support team depending on a new tooling feature).

#### Responsibilities
- Provide detailed requirements from a day-to-day user perspective
- Participate in user acceptance testing (UAT)
- Give timely feedback on delivered features

#### Typical Communication
- Involvement in UAT and demo sessions
- Regular feedback loops with PM and Business Analyst
- Email or chat updates on delivery milestones

### External Partner

#### Role Summary
An external partner is an organization or vendor that integrates with OctoAcme systems or co-delivers parts of the project scope.

#### Responsibilities
- Fulfill contractual deliverables on agreed timelines
- Participate in integration testing and joint reviews
- Notify OctoAcme of changes that may affect integration points

#### Typical Communication
- Structured meeting cadence with PM (weekly or bi-weekly)
- Formal written communications for scope changes
- Shared integration test environment and defect logs

### Executive Sponsor

#### Role Summary
The Executive Sponsor has organizational authority over the project and is accountable for business outcomes. They remove escalation blockers and champion the project at the leadership level.

#### Responsibilities
- Approve project charter and major scope changes
- Unblock resource or organizational constraints
- Receive high-level status updates and escalation alerts

#### Typical Communication
- Monthly or milestone-based briefings
- Escalation calls when strategic decisions are needed
- Executive summary in release announcements

### Support / Operations

#### Role Summary
Support / Operations teams own the post-release customer experience and operational continuity. They need advance notice of changes that affect workflows, runbooks, or support scripts.

#### Responsibilities
- Review release notes for support impact
- Update runbooks and support scripts ahead of releases
- Report production incidents back to the delivery team
- Participate in post-release monitoring and feedback

#### Typical Communication
- Pre-release briefings with Release Manager
- Release notes review before publish
- Incident escalation channels for production issues

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
## Related Resources
- See also: [Handoff Checklist](./octoacme-handoff-checklist.md) and [RACI-Lite Ownership Map](./octoacme-roles-raci-lite.md) for artifact-level ownership guidance.

