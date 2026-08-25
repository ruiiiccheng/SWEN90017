# ADR-0001 — Select Application Architecture

**Status:** Proposed — final decision blocked by starter-repository audit  
**Decision owners:** Student development team, with Product Owner and lecturer input  
**Last updated:** 25 August 2026

## Context

The client described a PostgreSQL/Alembic CRM implemented in Python with server-rendered templates, limited API support and small embedded React lookups. Both FastAPI and Flask were mentioned, and the team has not yet inspected the intended public Bootstrap repository. React/Python and React/Go alternatives were discussed, but no replacement decision was made.

The architecture must deliver a coherent CRM vertical slice within the course schedule, remove Salesforce presentation/IP dependencies and leave a controlled boundary for later AI workflow integration.

## Options

| Option | Main benefit | Main risk |
|---|---|---|
| A. Extend Python + server-rendered Bootstrap | Maximum reuse and lowest initial delivery risk if the starter is coherent. | Inherited gaps or mixed framework boundaries may slow change. |
| B. React UI + Python API | Clear UI/API separation while retaining Python and potentially reusable domain/data code. | Additional front-end, API, authentication and integration work. |
| C. React UI + Go API | Clean replacement boundary and Go learning opportunity. | Highest rewrite and schedule risk; no demonstrated performance need. |

## Interim decision

The final stack remains undecided until the audit and spike are complete. Until then:

1. Evaluate the starter repository before discarding it.
2. Keep requirements, domain modelling and the low-fi prototype stack-neutral.
3. Do not begin a full React or Go rewrite solely for novelty.
4. Prefer the smallest architecture that can deliver and test the Sprint 1 Account–Contact–Task vertical slice.
5. Reuse PostgreSQL/Alembic only after their condition and fit are verified.

## Selection criteria

1. Ability to deliver the agreed MVP and vertical slice on time.
2. Amount and quality of verified reusable code and schema.
3. Team capability and integration risk.
4. Maintainability, testability and clear business-logic boundaries.
5. Reproducible local development and CI.
6. Suitability for the selected AI workflow without premature complexity.

## Evidence required before acceptance

- Complete [starter-repository-audit.md](starter-repository-audit.md).
- Run the same Account → Contact lookup/link → related Task flow from a clean checkout.
- Compare the leading options using a small implementation spike rather than feature-count assumptions.
- Record the selected option, rejected alternatives and concrete consequences here; then update decision `D-007`.

## Current consequence

No final `/frontend`, `/backend` or service split should be treated as approved. The current [architecture overview](architecture-overview.md) is a logical baseline, not an as-built diagram.
