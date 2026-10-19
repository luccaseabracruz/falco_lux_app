---
status: Draft
---
# M0 — Walking skeleton

## Outcome
The admin logs in to a staging environment over HTTPS, creates a site and a technician, and the system prevents the technician from using admin functions. From here on, delivering is a repeatable process.

## In scope
- Repository, linting and CI.
- Staging with HTTPS, database, migrations and secrets outside the code.
- Authentication and RBAC (admin / technician) **enforced on the server**.
- Site CRUD (name, coordinates, radius, IANA time zone).
- i18n mechanism PT/ES (translate later).
- Basic database backups.

## Out of scope
Clock-in, birds, offline, selfie, reports.

## Stories
- [ ] Repository + linting + green CI
- [ ] Deploy to staging with HTTPS
- [ ] Database + migrations
- [ ] Secrets management (nothing in the repository)
- [ ] Login/logout with secure passwords and secure sessions/tokens
- [ ] RBAC: admin vs. technician
- [ ] Site CRUD
- [ ] i18n structure
- [ ] Backup and restore test

## Success criteria
- Admin creates a site and a technician in staging.
- An automated test proves the technician gets 403 on admin routes.
- A backup restore was tested once.

## Definition of Done
Tests pass, CI green, deployed to staging, docs and ADRs updated, proportional security check (server-side authorization, validated input, no secrets in code).

## Risks and unknowns
- ADR-001 (client platform) may constrain the stack choice.
- OQ-01 (site vs. technician) affects the data model.
- First time with DevOps/CI/deploy: learning time.

## Required ADRs
ADR-001 (platform), stack/hosting choice (ADR-002).

## Estimate
~25-40 h (low confidence). Actual: _to fill._