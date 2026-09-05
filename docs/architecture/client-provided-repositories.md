# Client-Provided Reference Repositories

**Source:** repositories shared by the client (Peter Harding)  
**Recorded:** 31 August 2026

These repositories are reference material for the team's starter-repository and database-migration assessment. They are not yet confirmed as the authoritative CRM codebase.

| Repository | Known purpose | Relevance / follow-up |
| --- | --- | --- |
| [base-api](https://github.com/peterlharding/base-api) | A basic API implemented with FastAPI. | Review its project structure, endpoints, configuration and test approach as a possible API starting point. |
| [new-api](https://github.com/peterlharding/new-api) | Purpose not yet described in the client message. | Inspect the README, default branch and current state before relying on it. |
| [fastapi-db-schema](https://github.com/peterlharding/fastapi-db-schema) | Appears to contain FastAPI database-schema material; no further description was supplied. | Check its schema definitions, database connection setup and migration strategy. |
| [alembic-demo](https://github.com/peterlharding/alembic-demo) | Demonstrates using Alembic to version a PostgreSQL schema for API use, targeting a Docker-based PostgreSQL instance. | Use as a reference for local database setup and migration workflow. The client plans to add a branch demonstrating the CRM schema after it has been tidied. |

## Verification checklist

Before adopting any repository or branch, record:

- authoritative repository URL, default branch and inspected commit;
- licence and third-party dependencies;
- clean-checkout setup steps, environment variables and Docker services;
- implemented API, database schema and Alembic migration capabilities; and
- gaps relative to the CRM's accounts, contacts, leads, opportunities, tasks and events.

See [Starter Repository Architecture Audit](starter-repository-audit.md) for the broader evidence required before selecting the implementation baseline.
