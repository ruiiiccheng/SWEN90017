# Client Meeting 2 — Access, Architecture and Sprint 1 Direction

**Date/time:** 26 August 2026; exact time not recorded  
**Attendees:** Peter Harding (PerformIQ) and Team 6 student members  
**Facilitator:** Peter Harding / Team 6  
**Note source:** Three-part automated transcript  
**Source quality:** Rough transcript; speaker attribution and some technical terms are uncertain. Credentials, email addresses and other personal identifiers have intentionally been omitted.

## Objectives

- Obtain access to the current hosted CRM and relevant reference repositories.
- Understand the current implementation and the client's suggested technical direction.
- Clarify how closely the new solution should follow the inherited interface.
- Agree on Sprint 1 priorities, documentation practices and the next client review.

## Demonstrated work

- Peter demonstrated the hosted CRM and provisioned access for the student team.
- Team members opened the system and began testing basic account, contact and task workflows.
- Peter walked through the current server-rendered Python application, its embedded React lookup components and the beginnings of its API.
- Peter showed newer API and database-schema repositories as reference material. A live authentication/API test returned errors and was not resolved during the recorded session.
- The team reported that it had started a React prototype and asked how closely its interface should resemble the inherited CRM.
- A Slack channel for repository links was created and reference links were shared during the meeting.

## Discussion and clarifications

### 1. Access and source repositories

- The hosted CRM is available for the team to explore using individually provisioned access.
- Peter plans to provide a cleaner Bootstrap-based copy of the application with the old Salesforce-specific presentation removed.
- Peter also showed private API and database-schema repositories. He clarified that these are examples and references, not components that the team is required to combine or adopt unchanged.
- The intended authoritative starter repository and branch were not conclusively identified in the transcript.

### 2. Current implementation and possible architecture

- The current application is primarily server-rendered and talks directly to PostgreSQL. It also includes early API endpoints and embedded React components for record lookups and relationships.
- The transcript describes the application as both FastAPI/Jinja and Flask-based at different points. The repository must therefore be inspected before the stack is recorded as fact.
- Peter's possible evolution path is to expand API coverage across the main tables and build a full React front end.
- The team is not required to preserve the current implementation. Peter explicitly allowed a rebuild and left the back-end language open, mentioning Python, Go and Rust as possible choices.
- Running the database and application locally with Docker was recommended. Because the course currently provides one repository, a monorepo containing front end, back end and tests is an acceptable structure.

### 3. Product exploration and requirements

- The team should first explore the inherited CRM and use its behaviour as evidence when drafting user stories.
- Work can be divided by functional area: accounts, contacts, leads, opportunities, and tasks/events.
- Personas, user stories and acceptance criteria should be drafted, reviewed with the client and updated as understanding improves.
- The current layout was considered a useful reference, but the client did not require an exact visual copy. The new interface should retain the main CRM features while the team may change styling, colour and presentation.

### 4. Data model and technical references

- The supplied schemas are starting references rather than a final approved data model.
- Peter discussed replacing legacy Salesforce-style references with UUIDs and conventional relational foreign keys.
- Composite or derived fields, such as formatted full names, may be implemented through SQLAlchemy hybrid properties rather than duplicated front-end logic.
- Address normalisation remains open. The existing account structure was considered adequate as a temporary starting point.
- Geographic, timesheet and goal-model examples shown during the walkthrough were illustrative material and were not proposed as CRM scope.

### 5. Delivery, documentation and communication

- The first technical target is to understand the system and get the API running reliably.
- Slack should be used for ongoing client conversation and repository access coordination, while durable requirements and decisions should be recorded as Markdown in the repository.
- Feature-level planning documents and an initial proposal should be created once the first requirements draft is ready. AI tools may assist with review, planning and code generation, but their output still requires team validation.
- Although the overall project spans two subjects, the team expects to deliver a working increment by the end of the current semester. The exact semester-one scope still needs to be made explicit.
- Peter expected to be unavailable the following week and suggested a progress or sprint presentation in the subsequent week.

## Decisions

| ID | Decision | Owner | Date | Affected stories/docs |
|---|---|---|---|---|
| CM2-D01 | Treat the inherited application and the newer schema/API repositories as evidence and reference material, not as a mandatory final architecture. | Team 6 | 2026-08-26 | Architecture spike; repository audit |
| CM2-D02 | Explore the current CRM before finalising user stories, dividing analysis across accounts, contacts, leads, opportunities, and tasks/events. | Team 6 | 2026-08-26 | Personas; user stories; product backlog |
| CM2-D03 | Preserve the main CRM capabilities and information flow, while allowing the React prototype to use its own visual styling. | Team 6 | 2026-08-26 | Prototype; UI requirements |
| CM2-D04 | Prioritise getting the API running and understanding the inherited architecture before making a final stack decision. | Team 6 | 2026-08-26 | Sprint 1; architecture spike |
| CM2-D05 | Use Slack for active client communication and keep durable feature and decision documentation in the repository. | Team 6 / Peter | 2026-08-26 | Communication; project documentation |

## Actions

| ID | Owner | Action | Due | Status |
|---|---|---|---|---|
| CM2-A01 | Peter Harding | Provide access to the cleaned Bootstrap/front-end repository after removing legacy Salesforce-specific material. | By the end of the meeting week (28 August 2026) | Open |
| CM2-A02 | Peter Harding | Complete or clarify access to the private API and database-schema reference repositories. | As soon as available | In progress |
| CM2-A03 | Team 6 | Explore the hosted CRM using sample accounts, contacts, tasks and related records; document observed working, partial and missing behaviour. | Sprint 1 | In progress |
| CM2-A04 | Team 6 | Divide the core CRM areas among team members and draft personas, user stories and initial acceptance criteria. | End of Sprint 1 | Planned |
| CM2-A05 | Technical team | Inspect the supplied repositories, verify the actual framework and dependencies, and attempt a reproducible local/Docker setup. | End of Sprint 1 | Planned |
| CM2-A06 | Technical team / Peter Harding | Diagnose the authentication/API errors observed during the live demonstration. | Before the next technical review | Open |
| CM2-A07 | Team 6 | Continue the React prototype using the inherited system's main functions as reference without copying its visual design exactly. | Next sprint review | In progress |
| CM2-A08 | Team 6 | Prepare a progress demonstration covering the prototype, API status, repository findings, user stories and draft acceptance criteria. | Next client-attended session | Planned |

## Risks/blockers

- **Repository readiness:** The cleaned application repository and complete front-end source were not yet available during the meeting.
- **API/authentication failure:** The live API authentication attempt produced server and invalid-user errors, so the reference API was not demonstrated end to end.
- **Stack ambiguity:** The transcript alternates between FastAPI/Jinja and Flask terminology; architecture decisions should wait for direct code inspection.
- **Scope ambiguity:** The working semester-one increment and its acceptance criteria have not yet been approved.
- **Source sensitivity:** The raw transcript contains access credentials and personal information. It should be redacted before being committed or shared; none of those values are reproduced in these minutes.

## Questions requiring client answer

- Which repository and branch should be treated as the authoritative starter code once the cleaned version is available?
- What minimum authentication and role-management behaviour is required for the semester-one deliverable?
- Which core workflows and acceptance criteria must be included in the first working increment?
- Is React plus the inherited Python API the preferred baseline after the repository audit, or should the team select freely based on the architecture spike?
- Which product-facing AI workflow should be implemented first, and what human-approval boundary is expected?
- What is the confirmed date and expected scope of the next client-attended demonstration?

## Excluded / unrelated transcript material

The following passages are not CRM requirements, project decisions or delivery actions:

| Source passage | Classification | Treatment in these minutes |
|---|---|---|
| `client_meeting-2-part2_transcript.txt`, approximately lines 155–160: a student explains an iOS expense-tracking app that lets a group share expenses. | **Unrelated — student side project discussion** | Excluded from CRM scope, requirements, decisions and actions. |
| `client_meeting-2-part2_transcript.txt`, approximately lines 226–258: peer conversation about AI-tool subscriptions, API pricing and another possible app. | **Unrelated — informal peer discussion** | Excluded from the meeting outcomes. |
| `client_meeting-2-part1_transcript.txt`, approximately lines 52–64: FreeCAD, 3D printing hardware and running a local language model. | **Unrelated — client tangent** | Excluded from CRM scope. |
| `client_meeting-2-part1_transcript.txt`, approximately lines 367–387 and 424–430: geographic, timesheet and goal-model schema examples. | **Reference-only, outside current CRM scope** | Mentioned only to prevent the examples from being mistaken for requirements. |
| Account creation, credential handling and the detailed live debugging dialogue across parts 1–3. | **Administrative/technical session detail** | Summarised at outcome level; all credential and identity values omitted. |

## Next meeting

- **Date/time:** Exact date TBD; Peter indicated that he would be away the following week and available in the subsequent week.
- **Expected demonstration:** Current React prototype, API/local-environment status, starter-repository audit findings, and draft user stories with acceptance criteria.
