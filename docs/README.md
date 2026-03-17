# OctoAcme Project Management Docs

## Overview

OctoAcme runs projects through a structured, end-to-end lifecycle: **Initiation → Planning → Execution → Release → Close & Retrospective**. During initiation, teams validate the business need, define measurable outcomes, identify stakeholders, outline a rough timeline, and capture early risks—typically in a **Project One-pager/Charter** (covering problem statement, SMART objective, success metrics, stakeholders, milestones, risks, and proposed roles). Once success metrics are agreed upon and team capacity is confirmed, the work advances through a go/no-go decision gate into planning. In planning, the approved initiative is broken into shippable increments with a prioritized backlog, acceptance criteria, a Definition of Done, a release plan, and an explicit **Risk Register** (tracking impact, likelihood, owner, mitigation, and status).

Day-to-day execution centers on a project board (Backlog → Ready → In Progress → In Review → QA → Done) and a pull request workflow optimized for fast, safe delivery: small PRs where possible, issue links and acceptance criteria in PR descriptions, CI checks before review, and at least one approval before merge per team policy. Risks and cross-team dependencies identified in planning are revisited regularly and escalated when needed—from team-level standup triage, to PM/Product Lead coordination, to sponsor-level escalation for business-impacting issues.

Each project includes defined **roles and responsibilities**: the Project Manager (PM) coordinates delivery, schedules, risk, and communications; the Product Manager (PdM/Product Lead) owns the product vision, prioritizes the backlog, and measures outcomes; Developers implement and test features; QA/Testing validates acceptance criteria and quality standards; and Stakeholders provide inputs and approvals. Communication follows a consistent cadence—daily standups for blockers and dependencies, a weekly delivery sync to surface progress and risks, regular demos at sprint or milestone boundaries, and monthly stakeholder updates—supported by a single source of truth for status (project README or release doc).

**Quality assurance and release practices** are built into every phase: teams write unit tests for new logic, add integration tests where applicable, and run end-to-end smoke tests for critical flows before each release. Security scanning runs in CI, and manual QA is applied when needed for feature acceptance. Releases (patch, minor, or major) follow a pre-release checklist—acceptance criteria met, CI and security scans passing, release notes drafted, rollback plan documented, smoke tests prepared—and a deployment checklist that covers staging validation, post-deploy verification, and stakeholder announcements. After sprints, releases, milestones, and incidents, OctoAcme holds retrospectives to capture what went well, identify improvements, and convert the top action items into owned, time-bound backlog work reviewed in ongoing PM/product syncs.

---

## Index

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | Principles, core roles, key artifacts, lifecycle summary, and communication cadence |
| [Project Initiation](octoacme-project-initiation.md) | Steps to validate and authorize work, one-pager template, and initiation checklist |
| [Project Planning](octoacme-project-planning.md) | Turning an approved initiative into a backlog, release plan, and milestone map |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Day-to-day team rhythm, PR workflow, quality/testing standards, and escalation levels |
| [Risks & Communication](octoacme-risks-and-communication.md) | Risk register format, risk lifecycle, stakeholder communication, and escalation paths |
| [Release & Deployment](octoacme-release-and-deployment.md) | Release types, pre-release requirements, deployment checklist, and rollback playbook |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Retrospective structure, running sessions, tracking improvements, and action item template |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed responsibilities, goals, and communication norms for Developers, Product Managers, and Project Managers |
