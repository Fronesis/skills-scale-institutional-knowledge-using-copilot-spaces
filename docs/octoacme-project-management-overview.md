# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
The following roles appear across OctoAcme projects. Full definitions, responsibilities, goals, and cross-role interactions are in [Roles & Personas](./octoacme-roles-and-personas.md).

**Always present:**
- Project Manager (PM): coordinates delivery, schedules, risk, communications.
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success.
- Developers: implement features, collaborate on design and testability.

**Added based on project scope:**
- QA Lead: owns test strategy, quality gates, and release readiness sign-off.
- QA / Testing: executes test cases and validates features during development.
- UX Designer: designs user flows and screens; validates usability.
- Release Manager: manages release calendar, windows, and cross-functional coordination.
- DevOps / Platform Engineer: maintains CI/CD pipelines, infrastructure, and deployment tooling.
- Business Analyst: gathers and refines requirements; bridges stakeholders and delivery team.
- Stakeholders: provide inputs and approvals. Subtypes include Internal Customer, External Partner, Executive Sponsor, and Support / Operations.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items
- [Handoff Checklist](./octoacme-handoff-checklist.md): cross-functional sign-offs at each phase transition
- [RACI-Lite Ownership Map](./octoacme-roles-raci-lite.md): lightweight artifact ownership reference

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
