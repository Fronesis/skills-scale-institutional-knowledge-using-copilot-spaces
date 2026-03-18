# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (verified by **DevOps / Platform Engineer**)
- Release notes drafted and reviewed (owned by **Release Manager**, input from PdM and Developers)
- Rollback / mitigation plan documented (owned by **Release Manager** in coordination with **DevOps**)
- Smoke tests prepared and executed (owned by **QA Lead**)
- Quality gate sign-off from **QA Lead** (see [Handoff Checklist](./octoacme-handoff-checklist.md#3-qa--release-handoff-qa-lead--release-manager))

## Deployment Checklist
- [ ] Deployment window scheduled by **Release Manager** (if needed)
- [ ] Backup or snapshot (if applicable) — coordinated by **DevOps**
- [ ] Deploy to staging and run smoke tests — **DevOps** deploys, **QA Lead** validates
- [ ] Deploy to production (automated pipeline preferred) — owned by **DevOps / Platform Engineer**
- [ ] Run post-deploy verifications — **QA Lead** and **DevOps**
- [ ] Announce release to stakeholders and support — **Release Manager** (see [Handoff Checklist](./octoacme-handoff-checklist.md#4-release--support--operations-handoff-release-manager--support-lead))

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

## Related Documents
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [Handoff Checklist](./octoacme-handoff-checklist.md)
- [RACI-Lite Ownership Map](./octoacme-roles-raci-lite.md)
