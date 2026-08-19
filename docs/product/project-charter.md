# Project Charter — AI-enabled CRM

**Status:** Draft for product-owner validation  
**Prepared:** 5 August 2026

## Product vision

For small or specialised organisations that need a flexible way to manage customers, prospects, sales activities and repeatable workflows, the product will provide an AI-enabled CRM with a clear core data model and controlled agent-assisted workflows. Unlike a legacy screen clone, it will prioritise coherent end-to-end workflows, traceable activity history, configurable automation and a clean, maintainable implementation.

## Problem statement

The inherited CRM preserves useful records and demonstrates a broad Salesforce-inspired schema, but it contains incomplete functions, placeholders, legacy presentation/IP concerns and no settled AI workflow. The student team needs to turn that starting point into a deliberately scoped, testable product rather than reproducing every historical screen.

## Primary stakeholders

| Stakeholder | Proposed role | Notes |
|---|---|---|
| Peter Harding, PerformIQ | Primary client / provisional Product Owner | Confirm whether Peter has final backlog and acceptance authority. |
| William Holt | Client/domain contributor | Provides specialised service-business and sales scenarios. |
| Leon | Lecturer / academic stakeholder | Reviews process, requirements and project progress. |
| Student team | Scrum developers | Own discovery, design, implementation, testing and documentation. |
| Scrum Master | Team member or rotation | Team to nominate. |

## Proposed product outcomes

1. A working CRM vertical slice covering the six initial schema areas.
2. Correct relationships between organisations, people, prospects, sales opportunities and activities.
3. A usable activity history that supports customer context and follow-up.
4. At least one controlled, auditable AI-assisted workflow that delivers demonstrable user value.
5. A documented, testable and reproducible codebase with no Salesforce visual/IP dependency.
6. A backlog and architecture plan that make incomplete or future work explicit.

## Proposed success criteria

- A new team member can run the application from a clean checkout using repository instructions.
- A user can create an account, add a linked contact, capture a lead, create an opportunity, schedule a task/event and see those activities in context.
- The selected AI workflow can be configured or drafted, executed, reviewed by a human where consequential, and audited.
- Automated tests cover the selected critical flows and all accepted stories meet the Definition of Done.
- The Product Owner accepts the agreed demonstration scenarios.
- The UI and assets are independent of Salesforce branding and copied look-and-feel.

## Constraints

- Course schedule, team capacity and sprint cadence are not yet documented.
- Starter repository access and exact technology state are dependencies.
- The transcript is imperfect and must not be treated as a complete specification.
- AI use introduces privacy, security, observability and human-control requirements.
- Architecture learning goals must be balanced against delivery risk.

## Non-goals for the initial MVP

Unless the Product Owner explicitly reprioritises them, the initial MVP will not attempt to reproduce the entire Salesforce feature set, Salesforce visual design, enterprise-scale organisational hierarchy, proposals/solutions, cases/contracts, advanced analytics, full route optimisation or every industry-specific workflow.
