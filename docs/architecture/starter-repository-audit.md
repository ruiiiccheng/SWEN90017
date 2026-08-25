# Starter Repository Architecture Audit

**Status:** Blocked — client repository access and walkthrough are pending (`I-04`)  
**Purpose:** Collect evidence required to update the architecture overview and close ADR-0001.

## Evidence checklist

| Area | Evidence to capture |
|---|---|
| Repository | Authoritative URL, licence, default branch and inspected commit. |
| Startup | Clean-checkout commands, required services, environment variables and seed data. |
| Frameworks | Actual FastAPI/Flask/Jinja/React/Bootstrap usage and package boundaries. |
| Data | PostgreSQL schema, Alembic history, legacy fields and migration health. |
| Capability | Working, partial, placeholder and missing features for the six core entities. |
| API | Routes, schemas, validation, authentication and error handling. |
| Quality | Tests, linting, CI, logging, security controls and dependency condition. |
| Deployment | Current local topology and whether Docker assets actually exist. |

## Required vertical trace

Trace one end-to-end flow through UI, server/API, domain logic and database:

> Create Account → create/link Contact through lookup → create related Task → view the connected record/history.

## Completion criteria

- Two team members can run the same inspected commit from a clean checkout.
- A concise working/partial/missing capability map is recorded.
- The as-built stack and boundaries replace uncertain claims in `architecture-overview.md`.
- ADR-0001 selects an implementation option or records a constrained interim decision.
- Relevant RAID issues and open questions are updated.
