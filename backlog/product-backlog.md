# Initial Product Backlog

**Status:** Draft for refinement and team estimation  
**Important:** Priorities and releases are a proposed starting point. The Product Owner owns ordering; the development team owns estimates.

## Summary

| ID | Epic | Title | Priority | Evidence | Proposed release |
| --- | --- | --- | --- | --- | --- |
| DISC-01 | Discovery and product definition | Benchmark representative CRM products | Must | Confirmed | Sprint 0 |
| DISC-02 | Discovery and product definition | Audit the starter CRM repository | Must | Confirmed | Sprint 0 |
| DISC-03 | Discovery and product definition | Confirm the MVP and reference business context | Must | Confirmed need; decision pending | Sprint 0 |
| DISC-04 | Discovery and product definition | Create a CRM data dictionary | Must | Confirmed | Sprint 0 |
| DEL-01 | Delivery enablement | Establish GitHub workflow and project memory | Must | Confirmed | Sprint 0 |
| DEL-02 | Delivery enablement | Create a reproducible local environment and CI baseline | Must | Proposed from transcript architecture discussion | Sprint 0 |
| DEL-03 | Delivery enablement | Provide safe demonstration data | Should | Proposed quality control | Sprint 0 |
| DEL-04 | Delivery enablement | Select the implementation architecture | Must | Confirmed options; decision pending | Sprint 0 |
| ACC-01 | Accounts and contacts | Create and maintain accounts | Must | Confirmed | MVP 1 |
| CON-01 | Accounts and contacts | Create and maintain contacts | Must | Confirmed | MVP 1 |
| CON-02 | Accounts and contacts | Link contacts to accounts | Must | Confirmed | MVP 1 |
| ACC-02 | Accounts and contacts | Search accounts and contacts | Must | Confirmed through lookup demonstrations | MVP 1 |
| ACC-03 | Accounts and contacts | View a connected customer record | Must | Confirmed | MVP 1 |
| ACC-04 | Accounts and contacts | Warn about likely duplicate records | Should | Proposed | MVP 2 |
| LEAD-01 | Leads and qualification | Create and maintain leads | Must | Confirmed | MVP 1 |
| LEAD-02 | Leads and qualification | Represent a lead from an existing or new organisation | Must | Confirmed | MVP 1 |
| LEAD-03 | Leads and qualification | Qualify or disqualify a lead | Must | Confirmed concept; statuses pending | MVP 1 |
| LEAD-04 | Leads and qualification | Convert a qualified lead | Should | Proposed from described flow | MVP 2 |
| OPP-01 | Opportunities and pipeline | Create and maintain opportunities | Must | Confirmed | MVP 1 |
| OPP-02 | Opportunities and pipeline | Validate expected close date | Must | Confirmed | MVP 1 |
| OPP-03 | Opportunities and pipeline | Progress opportunities through sales stages | Must | Confirmed concept; stage list pending | MVP 1 |
| OPP-04 | Opportunities and pipeline | See opportunity relationships and activities | Must | Confirmed | MVP 1 |
| OPP-05 | Opportunities and pipeline | Filter and review the sales pipeline | Should | Proposed CRM capability | MVP 2 |
| ACT-01 | Tasks, events and history | Create and maintain related tasks | Must | Confirmed | MVP 1 |
| ACT-02 | Tasks, events and history | Create and maintain related events | Must | Confirmed | MVP 1 |
| ACT-03 | Tasks, events and history | Display a unified activity timeline | Must | Confirmed gap and desired behaviour | MVP 1 |
| ACT-04 | Tasks, events and history | Record interaction notes | Must | Confirmed intent | MVP 1 |
| ACT-05 | Tasks, events and history | Review tasks and events in list/calendar views | Should | Confirmed list concept; calendar enhancement proposed | MVP 2 |
| ACT-06 | Tasks, events and history | Notify customers and users about scheduled work | Could | Optional service-domain requirement | Later |
| AI-01 | AI-enabled workflows | Define a workflow | Must | Confirmed objective; details pending | MVP 2 |
| AI-02 | AI-enabled workflows | Draft a workflow from natural-language instructions | Should | Proposed interpretation of project objective | MVP 2 |
| AI-03 | AI-enabled workflows | Execute and monitor a workflow | Must | Confirmed objective; details pending | MVP 2 |
| AI-04 | AI-enabled workflows | Require human approval for consequential AI actions | Must | Proposed safety requirement | MVP 2 |
| AI-05 | AI-enabled workflows | Summarise customer interaction history | Should | Proposed high-value use case | MVP 2 |
| AI-06 | AI-enabled workflows | Suggest or create a follow-up task from context | Should | Proposed high-value use case | MVP 2 |
| AI-07 | AI-enabled workflows | Use approved workflow templates | Could | Proposed | Later |
| AI-08 | AI-enabled workflows | Optimise a field-service day plan | Could | Optional domain example | Later |
| SEC-01 | Security and administration | Authenticate users | Must | Confirmed gap | MVP 1 or 2 |
| SEC-02 | Security and administration | Authorise by role | Must | Confirmed gap | MVP 2 |
| SEC-03 | Security and administration | Manage user accounts | Should | Confirmed need at concept level | MVP 2 |
| SEC-04 | Security and administration | Audit data and workflow changes | Must | Proposed quality requirement | MVP 2 |
| SEC-05 | Security and administration | Control CRM data sent to AI services | Must | Proposed safety requirement | Before AI production use |
| NFR-01 | Quality attributes | Use the CRM on common screen sizes | Should | Confirmed concern | MVP 2 |
| EXT-01 | Extensions | Create a quote from an opportunity | Should | Confirmed existing concept; not in initial schema brief | Later or MVP 2 |
| EXT-02 | Extensions | Attach documents to CRM records | Could | Confirmed concept; implementation absent | Later |
| EXT-03 | Extensions | Run basic reports and exports | Could | Existing placeholders mentioned; requirements unclear | Later |
| EXT-04 | Extensions | Manage cases or contracts | Won’t in initial MVP | Optional future concept | Future |

## Detailed backlog

## DISC-01 — Benchmark representative CRM products

    **Epic:** Discovery and product definition  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** Sprint 0  
    **Source trace:** Transcript 51-71 and 823-829  
    **Dependencies:** None identified

    **User story**  
    As the product team, I want to compare representative CRM products and their commonly used features, so that we can make evidence-based scope decisions rather than copying the inherited interface.

    **Acceptance criteria**
    - [ ] The team agrees an evaluation matrix covering core records, sales workflow, activities, security, reporting, integrations and AI capabilities.
- [ ] Each team member reviews one or two agreed CRM products and records findings in the shared repository.
- [ ] The team produces a consolidated feature map and identifies the gap between the starter system and the proposed MVP.

**Notes:** The comparison set is deliberately not fixed in this draft; the client mentioned Salesforce, Zoho and SugarCRM as examples.

## DISC-02 — Audit the starter CRM repository

    **Epic:** Discovery and product definition  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** Sprint 0  
    **Source trace:** Transcript 29-55, 101-107, 176-208 and 456-473  
    **Dependencies:** Access to Peter’s public Bootstrap repository

    **User story**  
    As the development team, I want to run and inspect Peter’s starter CRM and classify each capability as working, partial, placeholder or missing, so that we can reuse valuable code without assuming incomplete screens are functional.

    **Acceptance criteria**
    - [ ] A new developer can run the application using documented steps.
- [ ] The audit inventories screens, APIs, database tables, migrations, tests and known defects.
- [ ] Every inherited feature is marked working, partial, placeholder, missing or intentionally excluded.
- [ ] Any Salesforce branding, copied visual assets or look-and-feel dependencies are identified for removal.

## DISC-03 — Confirm the MVP and reference business context

    **Epic:** Discovery and product definition  
    **Priority:** Must  
    **Evidence status:** Confirmed need; decision pending  
    **Proposed release:** Sprint 0  
    **Source trace:** Transcript 496-504 and 711-829  
    **Dependencies:** Product-owner decision

    **User story**  
    As the product owner, I want to select the MVP outcome and a reference business context, so that the team can prioritise a coherent product instead of building a generic collection of screens.

    **Acceptance criteria**
    - [ ] The product owner confirms whether the MVP is a generic sales CRM, a service-business CRM, or a generic core demonstrated through a specific vertical.
- [ ] The agreed MVP explicitly lists in-scope, out-of-scope and later capabilities.
- [ ] The team records measurable acceptance outcomes for the end-of-project demonstration.

## DISC-04 — Create a CRM data dictionary

    **Epic:** Discovery and product definition  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** Sprint 0  
    **Source trace:** Project background lines 1-4; Transcript 63-126 and 625-642  
    **Dependencies:** None identified

    **User story**  
    As the product team, I want to define each core entity, relationship, required field, status and business rule, so that developers and clients use the same terminology and validation rules.

    **Acceptance criteria**
    - [ ] The dictionary covers at least accounts, contacts, leads, opportunities, tasks and events.
- [ ] Relationships, cardinalities and ownership rules are documented.
- [ ] Required fields, validation rules and lifecycle statuses are marked as confirmed or awaiting product-owner confirmation.

## DEL-01 — Establish GitHub workflow and project memory

    **Epic:** Delivery enablement  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** Sprint 0  
    **Source trace:** Transcript 397-430 and 575-680  
    **Dependencies:** GitHub repository access

    **User story**  
    As the student team, I want to use a shared repository, individual branches and durable Markdown project memory, so that human and AI-assisted work remains coordinated and reviewable.

    **Acceptance criteria**
    - [ ] The repository has a protected main branch and a documented branch/PR convention.
- [ ] Each member has a documented skills/workflow or member-memory file using the provided template.
- [ ] Decisions, client answers and architectural changes are written to the repository rather than remaining only in chat.
- [ ] At least one teammate reviews every merge to main.

## DEL-02 — Create a reproducible local environment and CI baseline

    **Epic:** Delivery enablement  
    **Priority:** Must  
    **Evidence status:** Proposed from transcript architecture discussion  
    **Proposed release:** Sprint 0  
    **Source trace:** Transcript 447-450  
    **Dependencies:** Architecture choice may alter exact tooling

    **User story**  
    As a developer, I want to start the database, API and user interface using documented commands, so that the system behaves consistently across team laptops and pull requests.

    **Acceptance criteria**
    - [ ] A clean checkout can be started using one documented workflow.
- [ ] Database migrations run automatically or through a single documented command.
- [ ] CI performs at least formatting/linting and automated tests on pull requests.
- [ ] Secrets and local configuration are excluded from version control and represented by an example environment file.

## DEL-03 — Provide safe demonstration data

    **Epic:** Delivery enablement  
    **Priority:** Should  
    **Evidence status:** Proposed quality control  
    **Proposed release:** Sprint 0  
    **Source trace:** Inferred; transcript describes legacy client data  
    **Dependencies:** None identified

    **User story**  
    As the development team, I want to seed realistic synthetic CRM data, so that features can be tested and demonstrated without exposing client information.

    **Acceptance criteria**
    - [ ] The seed dataset contains linked examples for every MVP entity.
- [ ] No real personal or commercially sensitive client data is included.
- [ ] The dataset can be reset repeatably for tests and demonstrations.

## DEL-04 — Select the implementation architecture

    **Epic:** Delivery enablement  
    **Priority:** Must  
    **Evidence status:** Confirmed options; decision pending  
    **Proposed release:** Sprint 0  
    **Source trace:** Transcript 218-250, 431-450 and 745-757  
    **Dependencies:** Starter-code audit and team skills inventory

    **User story**  
    As the development team, I want to evaluate the inherited Python server-rendered approach, React with a Python API, and React with a Go API, so that the team commits to an architecture based on delivery risk, learning value and maintainability.

    **Acceptance criteria**
    - [ ] The team verifies the actual starter stack because the transcript references both FastAPI and Flask/Jinja-like rendering.
- [ ] A short spike evaluates reuse, team skills, delivery time, testing, deployment, API completeness and AI integration.
- [ ] The selected option and rejected alternatives are recorded in an architecture decision record.

## ACC-01 — Create and maintain accounts

    **Epic:** Accounts and contacts  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Project background line 4; Transcript 625-642  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to create, view, edit, list and archive an account representing an organisation or other entity, so that I can maintain the organisations with which the business interacts.

    **Acceptance criteria**
    - [ ] Account name is required and a stable unique identifier is generated.
- [ ] The user can view and edit account details and can archive an account without losing its history.
- [ ] Archived accounts are excluded from default active lists but remain retrievable by authorised users.

## CON-01 — Create and maintain contacts

    **Epic:** Accounts and contacts  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Project background line 4; Transcript 63-79 and 625-642  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to create, view, edit, list and archive an individual contact, so that I can maintain the people with whom the business communicates.

    **Acceptance criteria**
    - [ ] A contact can be created with a name and optional communication details.
- [ ] The user can view, edit and archive the contact.
- [ ] The contact page displays its related account when one is linked.

## CON-02 — Link contacts to accounts

    **Epic:** Accounts and contacts  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 63-79 and 625-642  
    **Dependencies:** ACC-01 and CON-01

    **User story**  
    As a CRM user, I want to link a contact to an existing account while allowing a contact to exist without one, so that the system represents organisations, sole traders and unassociated individuals correctly.

    **Acceptance criteria**
    - [ ] The account field supports lookup and selection of an existing active account.
- [ ] Multiple contacts can be linked to one account.
- [ ] A contact may be saved without an account when business rules permit it.
- [ ] Changing or removing the relationship does not delete either record.

## ACC-02 — Search accounts and contacts

    **Epic:** Accounts and contacts  
    **Priority:** Must  
    **Evidence status:** Confirmed through lookup demonstrations  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 21-27, 63-79 and 127-140  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to search accounts and contacts by partial identifying information, so that I can quickly find and link the correct record.

    **Acceptance criteria**
    - [ ] Search returns relevant active records by partial name and other agreed identifiers.
- [ ] Lookup results distinguish records sufficiently to avoid selecting the wrong organisation or person.
- [ ] The same lookup behaviour is reusable from related-record forms.

## ACC-03 — View a connected customer record

    **Epic:** Accounts and contacts  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 154-180  
    **Dependencies:** Core entity and activity stories

    **User story**  
    As a CRM user, I want to see an account or contact together with related contacts, opportunities, tasks, events and notes, so that I can understand the relationship and interaction history without navigating many disconnected pages.

    **Acceptance criteria**
    - [ ] The account view lists linked contacts and open activities.
- [ ] The contact view shows the linked account and its own activities.
- [ ] Related items link to their detail pages and respect access permissions.

## ACC-04 — Warn about likely duplicate records

    **Epic:** Accounts and contacts  
    **Priority:** Should  
    **Evidence status:** Proposed  
    **Proposed release:** MVP 2  
    **Source trace:** Inferred data-quality need  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to receive a warning when a likely duplicate account or contact is entered, so that the CRM avoids fragmented histories and unreliable reporting.

    **Acceptance criteria**
    - [ ] The system checks agreed matching fields before creating a record.
- [ ] The user can inspect possible matches and choose an existing record or continue with justification.
- [ ] The warning does not silently merge or discard data.

## LEAD-01 — Create and maintain leads

    **Epic:** Leads and qualification  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Project background line 4; Transcript 79-101  
    **Dependencies:** None identified

    **User story**  
    As a sales user, I want to record and update a potential customer or enquiry as a lead, so that new business interest is captured before it becomes an established account or opportunity.

    **Acceptance criteria**
    - [ ] The user can create, view, edit, list and archive a lead.
- [ ] A lead stores the person, organisation name when known, communication details and agreed source/status fields.
- [ ] Required fields and validation errors are clearly displayed.

## LEAD-02 — Represent a lead from an existing or new organisation

    **Epic:** Leads and qualification  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 85-104  
    **Dependencies:** ACC-01 and ACC-02

    **User story**  
    As a sales user, I want to link a lead to an existing account or record a new organisation name, so that both new prospects and new contacts within known organisations can be handled.

    **Acceptance criteria**
    - [ ] The user can search and select an existing account for the lead.
- [ ] The user can instead enter an organisation that does not yet exist as an account.
- [ ] The system makes the two states clear and does not create an account until the agreed conversion step.

## LEAD-03 — Qualify or disqualify a lead

    **Epic:** Leads and qualification  
    **Priority:** Must  
    **Evidence status:** Confirmed concept; statuses pending  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 101-125  
    **Dependencies:** Data dictionary approval

    **User story**  
    As a sales user, I want to move a lead through agreed qualification statuses and record the outcome, so that the team can distinguish actionable prospects from unqualified enquiries.

    **Acceptance criteria**
    - [ ] The product owner approves the lead statuses and required transition information.
- [ ] A user can update the status and add dated qualification notes.
- [ ] A disqualified lead requires an agreed reason and remains in history.

## LEAD-04 — Convert a qualified lead

    **Epic:** Leads and qualification  
    **Priority:** Should  
    **Evidence status:** Proposed from described flow  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 90-105  
    **Dependencies:** Accounts, contacts and opportunities

    **User story**  
    As a sales user, I want to convert a qualified lead into linked account, contact and opportunity records, so that validated interest can progress without re-entering information or creating duplicates.

    **Acceptance criteria**
    - [ ] The user reviews proposed account, contact and opportunity data before conversion.
- [ ] Existing account/contact records can be selected instead of creating duplicates.
- [ ] Conversion succeeds atomically or leaves the original data unchanged with a clear error.
- [ ] The converted lead retains links to the resulting records.

## OPP-01 — Create and maintain opportunities

    **Epic:** Opportunities and pipeline  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Project background line 4; Transcript 95-125  
    **Dependencies:** None identified

    **User story**  
    As a sales user, I want to create, view, edit, list and close a specific potential sale, so that the business can manage work that may result in an order.

    **Acceptance criteria**
    - [ ] An opportunity has a name, stage, expected close date and agreed relationship fields.
- [ ] The user can link the opportunity to an existing account and, where required, a contact.
- [ ] The user can view, edit and close the opportunity as won, lost or another approved terminal state.

## OPP-02 — Validate expected close date

    **Epic:** Opportunities and pipeline  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 107-115  
    **Dependencies:** OPP-01

    **User story**  
    As a sales user, I want to record when an order is expected and receive clear validation, so that the pipeline reflects the expected timing of sales.

    **Acceptance criteria**
    - [ ] Expected close date is required for active opportunities unless the product owner approves an exception.
- [ ] The form explains that the date represents the expected order/closure date.
- [ ] Invalid or inconsistent dates produce actionable validation messages.

## OPP-03 — Progress opportunities through sales stages

    **Epic:** Opportunities and pipeline  
    **Priority:** Must  
    **Evidence status:** Confirmed concept; stage list pending  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 101-125  
    **Dependencies:** Data dictionary approval

    **User story**  
    As a sales user, I want to update an opportunity through agreed prospecting, qualification and closing stages, so that the team can understand and manage the sales process consistently.

    **Acceptance criteria**
    - [ ] The product owner approves stage names, order and any required transition fields.
- [ ] The current stage is visible in lists and details.
- [ ] Stage changes are timestamped and retained in history.

## OPP-04 — See opportunity relationships and activities

    **Epic:** Opportunities and pipeline  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 154-180  
    **Dependencies:** OPP-01 and activity stories

    **User story**  
    As a sales user, I want to see the opportunity’s account, contact, tasks, events, notes and later quotes in one view, so that I can manage the sale with its complete context.

    **Acceptance criteria**
    - [ ] The detail view shows all related MVP records and open activities.
- [ ] Closed/completed activities remain available in the historical view.
- [ ] The user can create a related task, event or note from the opportunity context.

## OPP-05 — Filter and review the sales pipeline

    **Epic:** Opportunities and pipeline  
    **Priority:** Should  
    **Evidence status:** Proposed CRM capability  
    **Proposed release:** MVP 2  
    **Source trace:** Inferred from sales-oriented CRM discussion  
    **Dependencies:** None identified

    **User story**  
    As a sales user or manager, I want to filter opportunities by stage, expected close date, account and owner, so that I can focus follow-up effort and identify delayed work.

    **Acceptance criteria**
    - [ ] The opportunity list supports the agreed filters and sorting.
- [ ] Totals/counts are calculated from the filtered result when amount is in scope.
- [ ] The view clearly distinguishes active, won and lost opportunities.

## ACT-01 — Create and maintain related tasks

    **Epic:** Tasks, events and history  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Project background line 4; Transcript 126-149  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to create, assign, prioritise, update and complete a task linked to a CRM record, so that follow-up work is visible and accountable.

    **Acceptance criteria**
    - [ ] A task records subject, due date, priority, status, assignee and an agreed related record.
- [ ] The related record can be selected through lookup.
- [ ] The user can complete or cancel the task while preserving it in history.
- [ ] Open and overdue tasks are distinguishable in lists.

## ACT-02 — Create and maintain related events

    **Epic:** Tasks, events and history  
    **Priority:** Must  
    **Evidence status:** Confirmed  
    **Proposed release:** MVP 1  
    **Source trace:** Project background line 4; Transcript 149-176  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to schedule and update an event linked to a CRM record, so that meetings and other scheduled interactions are visible with their customer context.

    **Acceptance criteria**
    - [ ] An event records subject, start, end, status and an agreed related record.
- [ ] The system prevents an end time earlier than its start time.
- [ ] The user can update or cancel the event and its historical record remains visible.
- [ ] Recurrence is explicitly deferred unless selected for the MVP.

## ACT-03 — Display a unified activity timeline

    **Epic:** Tasks, events and history  
    **Priority:** Must  
    **Evidence status:** Confirmed gap and desired behaviour  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 167-179  
    **Dependencies:** ACT-01, ACT-02 and ACT-04

    **User story**  
    As a CRM user, I want to see dated tasks, events and interaction notes in one chronological history, so that I can understand what has happened and what is planned for a customer or sale.

    **Acceptance criteria**
    - [ ] The timeline combines relevant activity types in descending or ascending date order.
- [ ] Each item displays type, date/time, status, author/assignee and a link to details.
- [ ] Open and historical items are distinguishable.
- [ ] The timeline is available from at least account, contact and opportunity detail views.

## ACT-04 — Record interaction notes

    **Epic:** Tasks, events and history  
    **Priority:** Must  
    **Evidence status:** Confirmed intent  
    **Proposed release:** MVP 1  
    **Source trace:** Transcript 171-180  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to add a timestamped note after a call, meeting or other interaction, so that important context is retained for future users.

    **Acceptance criteria**
    - [ ] A note can be added from an agreed related record.
- [ ] The note stores author, timestamp and content and appears in the activity timeline.
- [ ] Editing or deleting a note follows the approved audit policy.

## ACT-05 — Review tasks and events in list/calendar views

    **Epic:** Tasks, events and history  
    **Priority:** Should  
    **Evidence status:** Confirmed list concept; calendar enhancement proposed  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 168-172  
    **Dependencies:** None identified

    **User story**  
    As a CRM user, I want to review upcoming and overdue activities across customers, so that I can plan my workload rather than opening each record separately.

    **Acceptance criteria**
    - [ ] Separate task and event lists show upcoming, overdue and completed/cancelled items.
- [ ] Filters include date range, assignee, status and related record where applicable.
- [ ] A calendar presentation is delivered only if selected during refinement.

## ACT-06 — Notify customers and users about scheduled work

    **Epic:** Tasks, events and history  
    **Priority:** Could  
    **Evidence status:** Optional service-domain requirement  
    **Proposed release:** Later  
    **Source trace:** Transcript 286-298  
    **Dependencies:** Email provider, security/privacy decision and ACT-02

    **User story**  
    As a service coordinator, I want to prepare and send or queue an approved notification for a scheduled visit, so that customers and assigned staff know when work is planned.

    **Acceptance criteria**
    - [ ] The user can generate a notification draft from an event and related contact data.
- [ ] The user reviews and confirms the content and recipients before sending.
- [ ] The CRM records delivery status or a clear failure state in the activity history.

## AI-01 — Define a workflow

    **Epic:** AI-enabled workflows  
    **Priority:** Must  
    **Evidence status:** Confirmed objective; details pending  
    **Proposed release:** MVP 2  
    **Source trace:** Project background lines 1-2; Transcript 392-425  
    **Dependencies:** AI/workflow scope decision and security model

    **User story**  
    As a CRM administrator, I want to define a workflow using a trigger, conditions, ordered steps and approval points, so that repeatable business processes can be configured rather than hard-coded.

    **Acceptance criteria**
    - [ ] A workflow has a name, description, trigger, optional conditions, actions, enabled state and version.
- [ ] The system validates incomplete or unsafe workflow definitions before activation.
- [ ] A workflow can be saved as draft, activated and disabled by an authorised user.

## AI-02 — Draft a workflow from natural-language instructions

    **Epic:** AI-enabled workflows  
    **Priority:** Should  
    **Evidence status:** Proposed interpretation of project objective  
    **Proposed release:** MVP 2  
    **Source trace:** Project background lines 1-2  
    **Dependencies:** AI-01 and approved model/provider

    **User story**  
    As a CRM administrator, I want to describe a desired process in plain language and receive a structured workflow draft, so that agent assistance reduces the effort needed to set up workflows.

    **Acceptance criteria**
    - [ ] The AI produces a draft using only supported triggers, conditions and actions.
- [ ] The draft identifies ambiguities and asks for missing required information within the product flow.
- [ ] Nothing is activated until an authorised user reviews and confirms the structured definition.

## AI-03 — Execute and monitor a workflow

    **Epic:** AI-enabled workflows  
    **Priority:** Must  
    **Evidence status:** Confirmed objective; details pending  
    **Proposed release:** MVP 2  
    **Source trace:** Project background lines 1-2; Transcript 408-425  
    **Dependencies:** AI-01

    **User story**  
    As a CRM administrator, I want to run or trigger an active workflow and inspect its status, so that automated work is observable and failures can be corrected.

    **Acceptance criteria**
    - [ ] A supported trigger creates a workflow run with a unique identifier.
- [ ] Each step records start time, end time, outcome and any error without exposing secrets.
- [ ] Failed runs are visible and can be retried only according to the agreed idempotency rules.

## AI-04 — Require human approval for consequential AI actions

    **Epic:** AI-enabled workflows  
    **Priority:** Must  
    **Evidence status:** Proposed safety requirement  
    **Proposed release:** MVP 2  
    **Source trace:** Inferred from AI-agent integration  
    **Dependencies:** Security and audit stories

    **User story**  
    As a CRM user, I want to review an AI-proposed change before it updates records, sends messages or creates commitments, so that AI assistance remains controlled and accountable.

    **Acceptance criteria**
    - [ ] The interface shows the proposed action, affected records and relevant source context.
- [ ] The user can approve, edit or reject the proposal.
- [ ] Rejection causes no external or data-changing side effect.
- [ ] The decision and final action are written to the audit log.

## AI-05 — Summarise customer interaction history

    **Epic:** AI-enabled workflows  
    **Priority:** Should  
    **Evidence status:** Proposed high-value use case  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 171-180 and 408-425  
    **Dependencies:** ACT-03, authentication and approved AI data policy

    **User story**  
    As a CRM user, I want to request a concise summary of recent activities for an account, contact or opportunity, so that I can prepare for an interaction without reading every historical entry.

    **Acceptance criteria**
    - [ ] The summary is generated from records the user is authorised to view.
- [ ] The response identifies the date range and links or references the underlying CRM records.
- [ ] The summary is clearly marked as AI-generated and does not alter source records.

## AI-06 — Suggest or create a follow-up task from context

    **Epic:** AI-enabled workflows  
    **Priority:** Should  
    **Evidence status:** Proposed high-value use case  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 126-149 and 408-425  
    **Dependencies:** ACT-01 and AI-04

    **User story**  
    As a CRM user, I want to receive a proposed follow-up task based on notes, events or opportunity state, so that important next actions are less likely to be missed.

    **Acceptance criteria**
    - [ ] The proposal includes subject, due date, priority, assignee and related record when inferable.
- [ ] Uncertain values are surfaced rather than invented silently.
- [ ] The user confirms or edits the proposal before a task is created.

## AI-07 — Use approved workflow templates

    **Epic:** AI-enabled workflows  
    **Priority:** Could  
    **Evidence status:** Proposed  
    **Proposed release:** Later  
    **Source trace:** Inferred from workflow objective  
    **Dependencies:** AI-01

    **User story**  
    As a CRM administrator, I want to start from approved workflow templates such as lead follow-up, overdue opportunity and meeting follow-up, so that common processes can be configured quickly and consistently.

    **Acceptance criteria**
    - [ ] Templates are versioned and identify required configuration values.
- [ ] Creating from a template produces an editable draft rather than an immediately active workflow.
- [ ] The template catalogue records owner and intended use.

## AI-08 — Optimise a field-service day plan

    **Epic:** AI-enabled workflows  
    **Priority:** Could  
    **Evidence status:** Optional domain example  
    **Proposed release:** Later  
    **Source trace:** Transcript 270-298  
    **Dependencies:** Confirmed vertical, geocoding/routing service, event duration and location data

    **User story**  
    As a service coordinator, I want to receive a proposed visit sequence based on location, expected duration and working-hour constraints, so that travel and overtime can be reduced for a service-business use case.

    **Acceptance criteria**
    - [ ] The coordinator selects candidate visits and supplies or confirms required constraints.
- [ ] The system returns a proposal with sequence, estimated travel/service time and any unassigned work.
- [ ] The coordinator can edit and approve the plan before events are changed.

## SEC-01 — Authenticate users

    **Epic:** Security and administration  
    **Priority:** Must  
    **Evidence status:** Confirmed gap  
    **Proposed release:** MVP 1 or 2  
    **Source trace:** Transcript 202-208  
    **Dependencies:** None identified

    **User story**  
    As an authorised user, I want to sign in and sign out securely, so that CRM information is not exposed to unauthorised people.

    **Acceptance criteria**
    - [ ] Unauthenticated users cannot access protected CRM data or actions.
- [ ] Credentials and sessions are handled using the selected framework’s secure mechanisms.
- [ ] Sign-out invalidates the active session or token.

**Notes:** For a local prototype, any temporary single-user mode must be explicitly approved and must not be used with real data.

## SEC-02 — Authorise by role

    **Epic:** Security and administration  
    **Priority:** Must  
    **Evidence status:** Confirmed gap  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 196-208  
    **Dependencies:** SEC-01

    **User story**  
    As a CRM administrator, I want to assign roles that control administrative and standard-user actions, so that users receive only the permissions needed for their work.

    **Acceptance criteria**
    - [ ] The product owner approves the initial role/permission matrix.
- [ ] Server-side checks enforce permission rules; hiding a button alone is insufficient.
- [ ] A denied action returns a clear, non-sensitive message and is auditable where appropriate.

## SEC-03 — Manage user accounts

    **Epic:** Security and administration  
    **Priority:** Should  
    **Evidence status:** Confirmed need at concept level  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 192-208  
    **Dependencies:** SEC-01 and SEC-02

    **User story**  
    As a CRM administrator, I want to create, deactivate and assign roles to users, so that access remains current as the organisation changes.

    **Acceptance criteria**
    - [ ] An administrator can create and deactivate a user without deleting historical authorship.
- [ ] Role changes take effect according to the approved session policy.
- [ ] The system prevents removal of the final active administrator.

## SEC-04 — Audit data and workflow changes

    **Epic:** Security and administration  
    **Priority:** Must  
    **Evidence status:** Proposed quality requirement  
    **Proposed release:** MVP 2  
    **Source trace:** Inferred from multi-user and AI requirements  
    **Dependencies:** Authentication and AI workflow implementation

    **User story**  
    As an administrator or reviewer, I want to see who changed critical records or approved AI actions and when, so that the system is accountable and problems can be investigated.

    **Acceptance criteria**
    - [ ] The audit log records actor, timestamp, action, record/workflow identifier and outcome for agreed events.
- [ ] Sensitive values and secrets are not copied into audit messages.
- [ ] Ordinary users cannot alter audit records.

## SEC-05 — Control CRM data sent to AI services

    **Epic:** Security and administration  
    **Priority:** Must  
    **Evidence status:** Proposed safety requirement  
    **Proposed release:** Before AI production use  
    **Source trace:** Inferred from AI-enabled CRM objective  
    **Dependencies:** Client/university privacy decision and model/provider selection

    **User story**  
    As a product owner or administrator, I want to configure and document what CRM data may be processed by an AI provider, so that privacy, confidentiality and client expectations are respected.

    **Acceptance criteria**
    - [ ] The approved provider, data categories and retention assumptions are documented.
- [ ] The system sends only the minimum context needed for the selected AI task.
- [ ] Users are warned or blocked when a request would include data outside the approved policy.

## NFR-01 — Use the CRM on common screen sizes

    **Epic:** Quality attributes  
    **Priority:** Should  
    **Evidence status:** Confirmed concern  
    **Proposed release:** MVP 2  
    **Source trace:** Transcript 196-201 and 550-559  
    **Dependencies:** None identified

    **User story**  
    As a desktop or mobile user, I want to use core CRM workflows on common laptop, tablet and phone widths, so that field and office users can access the system without clipped or unusable layouts.

    **Acceptance criteria**
    - [ ] Core MVP pages have no horizontal clipping at agreed viewport widths.
- [ ] Forms, navigation and tables remain usable with keyboard and touch input.
- [ ] The team records supported browsers and viewport targets.

## EXT-01 — Create a quote from an opportunity

    **Epic:** Extensions  
    **Priority:** Should  
    **Evidence status:** Confirmed existing concept; not in initial schema brief  
    **Proposed release:** Later or MVP 2  
    **Source trace:** Transcript 157-167  
    **Dependencies:** Product-owner confirmation that quotes are in scope

    **User story**  
    As a sales user, I want to create and maintain a quote linked to an opportunity, so that a qualified sale can progress to a priced proposal.

    **Acceptance criteria**
    - [ ] A quote links to an opportunity and relevant account/contact records.
- [ ] The quote stores an agreed date, status and amount fields.
- [ ] Related tasks, events and history are visible from the quote.

## EXT-02 — Attach documents to CRM records

    **Epic:** Extensions  
    **Priority:** Could  
    **Evidence status:** Confirmed concept; implementation absent  
    **Proposed release:** Later  
    **Source trace:** Transcript 192-205  
    **Dependencies:** Storage, security and malware-scanning decisions

    **User story**  
    As a CRM user, I want to upload and retrieve documents associated with supported records, so that proposals, service material and other evidence remain with the customer context.

    **Acceptance criteria**
    - [ ] The product owner confirms allowed record types, file types and size limits.
- [ ] Authorised users can upload, download and remove or supersede a document according to policy.
- [ ] Metadata records uploader, date, filename and related record.

## EXT-03 — Run basic reports and exports

    **Epic:** Extensions  
    **Priority:** Could  
    **Evidence status:** Existing placeholders mentioned; requirements unclear  
    **Proposed release:** Later  
    **Source trace:** Transcript 186-201  
    **Dependencies:** Confirmed reporting questions and role model

    **User story**  
    As a manager or CRM user, I want to review and export agreed CRM summaries, so that the organisation can monitor activity and pipeline data outside individual records.

    **Acceptance criteria**
    - [ ] The product owner selects a small set of report questions before implementation.
- [ ] Reports use authorised data and clearly state filters/date ranges.
- [ ] Exports use an agreed safe format and do not expose fields the user cannot view in the application.

## EXT-04 — Manage cases or contracts

    **Epic:** Extensions  
    **Priority:** Won’t in initial MVP  
    **Evidence status:** Optional future concept  
    **Proposed release:** Future  
    **Source trace:** Transcript 319-324  
    **Dependencies:** None identified

    **User story**  
    As a future CRM user, I want to manage support cases or service contracts linked to customers, so that the CRM can later support post-sale service processes.

    **Acceptance criteria**
    - [ ] No implementation begins until a specific business process and product-owner priority are supplied.
- [ ] Any future design reuses the core account/contact/activity model where appropriate.
