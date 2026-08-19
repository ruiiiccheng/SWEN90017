# Client Discovery Meeting — Minutes

**Meeting date:** Not supplied  
**Prepared:** 5 August 2026  
**Source quality:** Automated/rough transcript; speaker attribution follows the roles supplied by the student team and is uncertain in short interjections.

## Attendees and roles

- **Peter Harding, PerformIQ** — primary client voice, demonstrated the inherited CRM and described requirements and technical options.
- **William Holt** — client/domain contributor, added service-business examples and operational requirements.
- **Leon** — lecturer, joined later, established the GitHub repository and reinforced the requirements-first process.
- **Student team** — asked clarification questions and will deliver the project.

## Purpose

Understand the inherited CRM, clarify the intended AI-enabled CRM project, establish an initial delivery approach, and set up collaboration.

## Discussion summary

### 1. Existing system

Peter demonstrated a sales-oriented CRM derived from an old Salesforce data model. The current implementation uses a PostgreSQL database and database versioning through Alembic; the transcript also references Python, FastAPI, Flask/server-side templating and small embedded React lookup components. The exact current stack must be verified from the repository rather than inferred from the recording.

The inherited application contains a mixture of working CRUD/list/detail functions, partially implemented functions and placeholders. A public Bootstrap-based version is intended to remove the Salesforce look and feel and any associated IP risk.

### 2. Core domain model

The core records are accounts, contacts, leads and opportunities, with tasks and events as related activities. An **account** represents an organisation or entity; a **contact** represents a person. Contacts usually link to accounts, while individuals may exist without an account and sole traders can make the distinction less visible.

A lead may represent a new organisation or a new person in an existing account. A qualified lead can progress toward a specific opportunity. An opportunity represents a potential sale and includes an expected close date — the date on which an order or sale is expected to close.

Tasks and events should link to customer/sales records. The CRM should retain interaction notes and a usable activity history rather than displaying only disconnected lists or placeholder sections.

### 3. Known gaps and possible extensions

The demonstration exposed missing or incomplete lookups, rendering defects, placeholder activity history, unimplemented quotes/proposals/solutions, limited reporting, no robust authentication, no role model and a flat user/organisation structure. Quotes and document attachments were discussed as plausible extensions; proposals, solutions, cases and contracts were not established as initial MVP requirements.

### 4. AI and workflow direction

The brief requires an AI-enabled CRM that integrates with agents for workflow setup and implementation. The meeting distinguished two possible uses of agents:

1. **Development collaboration:** individual AI-assisted workflows, Markdown project memory and a coordinating repository process.
2. **Product capability:** AI agents embedded in the CRM to assist or automate business workflows.

Both are relevant, but the first product-facing AI use case was not selected. This is a high-priority product-owner question.

### 5. Delivery and architecture

The client recommended starting with CRM research, requirements and a gap analysis before deciding how much inherited code to reuse. The team may start with Peter’s code but is not required to preserve it if another approach better meets the project goals.

Architecture options raised were:

- Extend the inherited Python/server-rendered Bootstrap application.
- Use React as the front end and Python/FastAPI as the API.
- Reimplement the API in Go and use React as the front end.

No option was selected. A time-boxed architecture spike is required.

### 6. Collaboration

GitHub was set up during the latter part of the meeting. Suggested practices include individual branches, Markdown memory files, shared planning documents and reviewable pull requests. The team had an internal WeChat group, but Slack was preferred for client-visible communication because it provides shared history. Material decisions should also be copied into the repository.

## Confirmed direction

- Start with requirements, user stories, CRM research and a starter-code gap analysis.
- Initial data model: accounts, contacts, leads, opportunities, tasks and events.
- Use a Bootstrap/non-Salesforce presentation and avoid Salesforce IP/look-and-feel reuse.
- Begin with Peter’s starter repository as evidence and a possible accelerator, not an immutable architecture.
- Use GitHub for source, planning and durable project memory.
- Use Slack for client-visible communication and weekly progress follow-up.
- Treat embedded AI/workflow automation as a major scope area requiring explicit refinement.

## Decisions not yet made

- Final Product Owner and acceptance authority.
- Generic CRM versus a specific reference vertical.
- Final architecture and level of starter-code reuse.
- First AI workflow and degree of autonomy.
- Authentication/roles delivery timing.
- Whether quotes, documents, email notifications, route optimisation and reports are in the MVP.
- Sprint duration and project milestone dates.

## Action register

| ID | Owner | Action | Due | Status | Basis |
| --- | --- | --- | --- | --- | --- |
| A-01 | Peter Harding | Provide access to the public Bootstrap-based CRM repository with Salesforce visual/IP elements removed. | Before code audit / next workshop | Open | Confirmed |
| A-02 | Peter Harding | Provide or demonstrate a running version and walk through the database schema, migrations, known gaps and API coverage. | Next available workshop | Open | Confirmed |
| A-03 | Student team | Send GitHub account details and verify repository access for every team member. | Immediately | Open | Confirmed |
| A-04 | Student team | Create/invite clients and lecturer to the agreed Slack channel; record material decisions there and in GitHub. | Immediately | Open | Confirmed |
| A-05 | Student team | Split CRM product research, complete individual summaries, and consolidate a feature/gap matrix. | Sprint 0 | Open | Confirmed |
| A-06 | Student team | Audit the starter system and classify working, partial, placeholder and missing functionality. | Sprint 0 | Open | Confirmed |
| A-07 | Student team + Product Owner | Refine and approve the initial user stories, MVP boundary and acceptance outcomes. | Sprint 0 review | Open | Confirmed need |
| A-08 | Student team | Run the architecture spike and record the selected stack in ADR-0001. | Sprint 0 | Open | Decision pending |
| A-09 | Peter Harding / William Holt | Confirm the reference business context and whether the service-route/field-knowledge scenario is core, a demonstration, or out of scope. | Sprint 0 review | Open | Proposed clarification |
| A-10 | Product Owner | Select the first embedded AI workflow use case and approve the human-approval/data-handling boundary. | Before AI implementation | Open | Proposed clarification |

## Transcript cautions

- The meeting date and some names/course identifiers are not clear enough to record as fact.
- The transcript alternates between FastAPI and Flask/server-rendered terminology; verify the repository.
- The spoken email address was mistranscribed; use the project-background address supplied separately.
- “Jinja” appears to have been transcribed as “Ginger”. This pack records the uncertainty rather than treating the correction as source fact.
