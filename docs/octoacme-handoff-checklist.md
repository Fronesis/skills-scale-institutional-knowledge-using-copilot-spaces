# OctoAcme — Cross-Functional Handoff Checklist

## Purpose
Ensure that critical context, artifacts, and sign-offs are explicitly transferred between teams at each project stage. Incomplete handoffs are a leading cause of rework, production incidents, and missed expectations.

## How to use
Complete each relevant checklist section when transitioning work between phases. The handoff owner is noted for each section. Attach completed checklists to the project board or link from the relevant milestone.

---

## 1. Product → Engineering Handoff (PdM → Dev Lead / QA Lead)

**Handoff owner:** Product Manager (PdM)  
**Completed before:** Sprint planning / development kickoff for a feature

- [ ] Feature specification or user story written with clear acceptance criteria
- [ ] Design files (wireframes / mockups) linked and finalized
- [ ] Business rules and edge cases documented (or Business Analyst sign-off)
- [ ] Success metrics defined and agreed with PM
- [ ] Dependencies on other teams or services identified
- [ ] Rollout constraints noted (feature flag, gradual rollout, region-specific)
- [ ] Any known risks or open questions captured in the Risk Register
- [ ] QA Lead briefed on scope and testability requirements

---

## 2. Engineering → QA Handoff (Dev Lead → QA Lead)

**Handoff owner:** Dev Lead (developers contribute items; the Dev Lead is accountable for ensuring all items are complete before signaling readiness)  
**Completed before:** QA begins testing on a feature branch or staging environment

- [ ] All acceptance criteria implemented and self-tested by developer
- [ ] PR merged (or marked ready-for-review) with passing CI checks
- [ ] Unit and integration tests written and passing
- [ ] Known limitations or deferred scope documented in the ticket
- [ ] Deployment instructions or environment configuration changes noted
- [ ] Test data or setup scripts provided if required
- [ ] QA Lead notified and build/branch location confirmed
- [ ] Linked issues and related PRs referenced in the handoff ticket

---

## 3. QA → Release Handoff (QA Lead → Release Manager)

**Handoff owner:** QA Lead  
**Completed before:** Release window is scheduled

- [ ] All test cases executed and results documented
- [ ] All blocker and critical defects resolved (or explicitly accepted risk noted)
- [ ] Regression suite passed on staging environment
- [ ] End-to-end smoke test results attached or linked
- [ ] Release readiness sign-off given by QA Lead
- [ ] Known issues list finalized for inclusion in release notes
- [ ] Test environment parity with production confirmed with DevOps
- [ ] Release Manager notified that QA gate is cleared

---

## 4. Release → Support / Operations Handoff (Release Manager → Support Lead)

**Handoff owner:** Release Manager  
**Completed before:** Release is published to production users

- [ ] Release notes published and linked
- [ ] Support team briefed on new features, changed behaviors, and known issues
- [ ] Runbooks and support scripts updated (or update tasks tracked)
- [ ] Rollback procedure documented and shared with on-call team
- [ ] Monitoring dashboards and alerts updated if needed (DevOps)
- [ ] Communication sent to internal stakeholders and/or customers
- [ ] Post-release monitoring window defined (e.g., 24-hour watch period)
- [ ] Escalation path for release-related incidents confirmed with on-call

---

## Related Documents
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [RACI-Lite Ownership Map](./octoacme-roles-raci-lite.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
