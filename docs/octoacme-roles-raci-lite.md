# OctoAcme — RACI-Lite Ownership Map

## Purpose
A lightweight, one-page reference showing who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for the most common project artifacts. Adapt this to your specific project at kickoff.

## RACI Key
| Code | Meaning |
|------|---------|
| **R** | Responsible — does the work |
| **A** | Accountable — owns the outcome; final decision-maker |
| **C** | Consulted — provides input before or during |
| **I** | Informed — receives updates after decisions are made |

> Roles referenced here are defined in [Roles & Personas](./octoacme-roles-and-personas.md).

---

## Artifact Ownership Table

| Artifact | PM | PdM | Dev Lead | QA Lead | UX Designer | Release Mgr | DevOps | Biz Analyst | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|
| **Project One-pager / Charter** | A | C | C | I | I | I | I | C | C |
| **Product Backlog** | C | A | C | C | C | I | I | R | I |
| **Sprint / Iteration Backlog** | R | C | A | C | I | I | I | I | I |
| **Acceptance Criteria** | C | A | C | C | C | I | I | R | C |
| **Definition of Done (DoD)** | C | A | R | R | C | C | C | I | I |
| **Design Files / Wireframes** | I | C | C | I | A/R | I | I | C | C |
| **Requirements / User Stories** | C | A | C | C | C | I | I | R | C |
| **Risk Register** | A/R | C | C | C | I | C | C | C | I |
| **Test Plan / Test Cases** | I | C | C | A/R | I | C | C | I | I |
| **Release Notes** | I | C | C | C | I | A/R | I | I | I |
| **Release Calendar** | C | C | I | C | I | A/R | C | I | I |
| **CI/CD Pipeline** | I | I | C | C | I | C | A/R | I | I |
| **Deployment / Rollback Plan** | I | I | C | C | I | A | R | I | I |
| **Retrospective Actions** | A/R | C | C | C | C | C | C | C | I |
| **Stakeholder Comms Updates** | A/R | C | I | I | I | C | I | C | I |
| **Incident Post-mortem** | A | I | C | C | I | C | R | I | I |
| **Handoff Checklist** | C | C | R (Eng→QA) | R (QA→Rel) | I | R (Rel→Sup) | C | I | I |

---

## Notes on Customization
- In smaller teams, one person may fill multiple roles. Ensure accountability (A) remains clearly assigned even when collapsed.
- For external partner involvement, add an "External Partner" column and assign **C** or **I** as appropriate.
- The Executive Sponsor is typically **I** for most artifacts but should be **C** or **A** for the Project Charter and major scope changes.
- **Backlog vs. Requirements**: The Product Backlog (row 3) shows PdM as Accountable and BA as Responsible because the BA writes and grooms items while the PdM owns backlog priority and direction. Requirements / User Stories (row 8) follows the same pattern. If your team's BA and PdM roles overlap significantly, consolidate accountability into one role.
- **Handoff Checklist ownership**: The Handoff Checklist row uses phase-specific R assignments (labeled in each cell) because responsibility changes hands at each stage. This differs from most artifacts where a single role is Responsible throughout the artifact lifecycle.

---

## Related Documents
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [Handoff Checklist](./octoacme-handoff-checklist.md)
- [Project Planning](./octoacme-project-planning.md)
- [Project Management Overview](./octoacme-project-management-overview.md)
