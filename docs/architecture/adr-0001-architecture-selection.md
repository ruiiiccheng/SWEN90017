# ADR-0001 — Select Application Architecture

**Status:** Proposed / decision pending  
**Decision owners:** Student development team, with Product Owner and lecturer input  
**Decision deadline:** End of Sprint 0

## Context

The inherited system appears to combine a PostgreSQL database, Alembic migrations, Python server-side rendering and small client-side lookup components. The transcript references both FastAPI and Flask/Jinja-like rendering, so the actual repository must be inspected. The meeting also raised React and Go as possible reimplementation choices.

The team needs an architecture that supports the course timeline, core CRM CRUD/relationships, controlled AI workflows, tests and local development without retaining Salesforce visual/IP dependencies.

## Options

### Option A — Extend the inherited Python/server-rendered Bootstrap application

**Advantages:** fastest reuse path if the code is coherent; lower rewrite risk; existing schema/migrations may be reusable.  
**Risks:** inherited placeholders and mixed architecture may slow change; API surface may be incomplete; modern interactive workflows may be harder.

### Option B — React front end + Python/FastAPI API

**Advantages:** separates UI/API, reuses Python knowledge and potentially existing API/domain code; suitable for interactive workflow UI.  
**Risks:** creates more moving parts; may require substantial API completion and front-end rebuild.

### Option C — React front end + Go API

**Advantages:** clear service boundary and Go learning opportunity; potentially strong static typing and deployment characteristics.  
**Risks:** highest rewrite/skill/schedule risk; may discard usable code; no evidence that CRM load requires a new backend language.

## Decision criteria and suggested weights

| Criterion | Weight |
|---|---:|
| Ability to deliver the agreed MVP on time | 30% |
| Reuse of verified working code/data model | 15% |
| Team capability and learning curve | 15% |
| Testability and maintainability | 15% |
| Support for AI/workflow integration | 10% |
| Local deployment and CI simplicity | 10% |
| Responsiveness and user experience | 5% |

## Spike tasks

1. Run the public starter repository from a clean checkout.
2. Trace one vertical flow: create account → contact lookup/link → related task.
3. Inventory API endpoints, templates/components, migrations and test coverage.
4. Implement or prototype the same smallest missing interaction in the leading options.
5. Score options against the agreed criteria and record evidence.

## Decision

Not yet made.

## Consequences to record after selection

- Repository structure and service boundaries.
- Data-access and migration strategy.
- Authentication/session approach.
- Front-end state/data-fetching approach.
- Workflow/agent integration boundary.
- Local Docker/development topology.
- Test strategy and deployment path.
