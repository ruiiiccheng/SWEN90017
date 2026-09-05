# RAID Log
**Review frequency:** Review during each Sprint Planning session and weekly team meeting.

A RAID Log records the project's:

- **Risks:** uncertain future events that may negatively affect the project.
- **Assumptions:** statements currently treated as true but requiring confirmation.
- **Issues:** problems that have already occurred and require resolution.
- **Dependencies:** external decisions, resources or actions required by the team.

## Assessment scale

Impact and likelihood are initial qualitative assessments and should be refined as more evidence becomes available.

### Impact

| Level | Meaning |
|---|---|
| High | Could prevent delivery, acceptance or safe operation of a major part of the product. |
| Medium | Could delay delivery or reduce quality, but a practical workaround may exist. |
| Low | Limited effect that can be handled through normal team processes. |

### Likelihood

| Level | Meaning |
|---|---|
| High | Expected to occur or already showing strong warning signs. |
| Medium | Could reasonably occur during the project. |
| Low | Unlikely, but still worth monitoring. |
| N/A | Not applicable to assumptions, current issues or dependencies. |

## Status values

| Type | Available statuses |
|---|---|
| Risk | Open, Monitoring, Mitigated, Materialised, Closed |
| Assumption | Unconfirmed, Confirmed, Invalidated |
| Issue | Open, In progress, Blocked, Resolved, Closed |
| Dependency | Pending, Available, Blocked, Complete |

## Risks

| ID | Type | Description | Impact | Likelihood | Response / next action | Owner | Review point | Status |
|---|---|---|---|---|---|---|---|---|
| R-01 | Risk | If the MVP and target vertical are not confirmed early, the team may implement features that do not meet Product Owner expectations. | High | High | Present an explicit in-scope, out-of-scope and later-scope proposal to the Product Owner and record the approved baseline. | Business analyst | Sprint 0 | Open |
| R-02 | Risk | Access to the starter repository may be delayed, or the repository may be incomplete or difficult to run. | High | Medium | This risk has materialised and is now managed through I-04. Continue non-dependent Sprint 0 work and maintain a clean-slate fallback. | Repo steward | Until I-04 is resolved | Materialised |
| R-03 | Risk | Inherited screens may appear complete while containing placeholders, incomplete workflows or broken links. | High | High | Complete a capability audit after repository access is granted. Add automated end-to-end smoke tests before deciding which inherited features can be reused. | Development team | Before reuse decisions | Open |
| R-04 | Risk | Reusing Salesforce branding, assets or distinctive interface designs may create intellectual-property concerns. | High | Medium | Create an independently designed Bootstrap-based interface. Remove Salesforce names, logos, copied assets and distinctive layouts. Record third-party licences and complete an IP review before release. | Repo steward | Before first release | Open |
| R-05 | Risk | A full React/Go rewrite may consume the available schedule before user value is delivered. | High | Medium | Conduct a time-boxed architecture spike and evaluate maintainability, team capability, migration effort and delivery risk. Require an end-to-end vertical-slice proof before approving a rewrite. | Technical lead | Architecture decision deadline | Open |
| R-06 | Risk | Different interpretations of “AI-enabled” may result in a deliverable that does not meet Product Owner expectations. | High | High | Separate team-agent coordination from embedded product functionality. Propose one product-level AI use case with defined inputs, outputs, controls and acceptance criteria for Product Owner approval. | AI lead | Sprint 0 | Open |
| R-07 | Risk | AI processing may expose personal or commercially sensitive CRM information. | High | Medium | Use synthetic development data, minimise model context, approve the AI provider and data boundary, protect secrets, require human approval for consequential actions and maintain an audit trail. | Security/AI lead | Before AI integration | Open |
| R-08 | Risk | Communication across WeChat, Slack, email and GitHub may cause decisions or requirements to be lost. | Medium | High | Use Slack and GitHub as durable sources of truth. Copy decisions, requirements and action items from informal channels into the appropriate repository document or issue. | Scrum Master | Weekly review | Open |
| R-09 | Risk | Team skill gaps in Go, React, FastAPI, PostgreSQL or the inherited Python stack may reduce development velocity. | Medium | Medium | Maintain a skills inventory, arrange pairing and code reviews, run targeted technical spikes and base architecture decisions on demonstrated team capability. | Technical lead | Sprint Planning | Open |
| R-10 | Risk | Route optimisation may expand into a separate and complex optimisation product. | High | Medium | Keep route optimisation outside the MVP or implement only a constrained pilot unless the Product Owner explicitly prioritises it and accepts the scope trade-off. | Business analyst | Scope review | Open |
| R-11 | Risk | The legacy data model may contain unnecessary fields, relationships or assumptions that make the new CRM harder to maintain. | Medium | High | Produce a simplified data dictionary, identify required business relationships and retain or migrate only fields approved for the MVP. | Data lead | Before schema implementation | Open |
| R-12 | Risk | Meeting transcripts may contain speech-recognition and speaker-attribution errors, resulting in incorrect requirements. | Medium | High | Validate uncertain statements through the open-question register, record requirement sources and evidence labels, and avoid treating uncertain transcript wording as confirmed fact. | Business analyst | Before baseline approval | Open |
| R-13 | Risk | Deferring authentication and role-based access may make the CRM unsuitable for multi-user use and prevent reliable attribution of record changes. | High | Medium | Define the minimum user-role and permission model before implementing protected APIs. Enforce authentication and authorisation on the server side. | Security lead | Before non-local deployment | Open |
| R-14 | Risk | The frontend, backend, database and AI components may work separately but fail during integration or deployment. | High | Medium | Deliver an early end-to-end vertical slice. Maintain CI, database migrations, environment documentation and deployment smoke tests. | Technical lead | First integration milestone | Open |
| R-15 | Risk | Limited Product Owner availability may delay requirement confirmation, repository access and acceptance decisions. | High | Medium | Maintain a prioritised question register, request asynchronous confirmation and set decision deadlines with clearly documented provisional assumptions. | Scrum Master | Weekly review | Open |
| R-16 | Risk | Critical project knowledge may become concentrated in one team member, causing delays when that person is unavailable. | Medium | Medium | Use pairing, code reviews, shared documentation and ownership rotation for critical components. | Scrum Master | Each Sprint retrospective | Open |

## Assumptions

| ID | Type | Description | Impact | Likelihood | Response / next action | Owner | Review point | Status |
|---|---|---|---|---|---|---|---|---|
| A-01 | Assumption | Peter Harding is the primary Product Owner and has final authority over scope, priorities and acceptance. | High | N/A | Ask Peter and the teaching team to confirm the Product Owner and final acceptance authority. Record the decision in the stakeholder register. | Scrum Master | Sprint 0 | Unconfirmed |
| A-02 | Assumption | Synthetic data can be used for all development, testing and product demonstrations. | High | N/A | Confirm data expectations, required import formats, representative data volume and whether any client-provided data will be needed. | Data lead | Before seed-data creation | Unconfirmed |
| A-03 | Assumption | The initial MVP can focus on a general sales CRM core, even if the demonstration uses a service-business context. | High | N/A | Present the proposed CRM core, target users and demonstration context to the Product Owner for confirmation. | Business analyst | Scope baseline review | Unconfirmed |
| A-04 | Assumption | Contacts may exist without being linked to an account, while active opportunities must be linked to an account. | Medium | N/A | Confirm the relationship and validation rules with the Product Owner before finalising the database schema. | Data lead | Before schema approval | Unconfirmed |
| A-05 | Assumption | AI-generated content will be treated as a draft and will require human approval before it changes CRM records or creates an external commitment. | High | N/A | Confirm the approval boundary for the selected AI workflow and document any explicitly permitted automatic actions. | AI lead | Before AI workflow implementation | Unconfirmed |

## Issues

| ID | Type | Description | Impact | Likelihood | Response / next action | Owner | Review point | Status |
|---|---|---|---|---|---|---|---|---|
| I-01 | Issue | The exact starter repository URL, licence and current working branch have not been confirmed. | High | N/A | Obtain access and record the repository URL, licence, default branch, active branch and relevant commit or release information. Do not copy or redistribute inherited code until its licence is understood. | Repo steward | Immediate | Open |
| I-02 | Issue | Sprint duration, project milestones and final delivery dates are not yet recorded in the project documentation. | High | N/A | Align the delivery plan with the course calendar and client availability. Record milestones, Sprint dates and review dates in the project plan. | Scrum Master | Before Sprint 1 | Open |
| I-03 | Issue | The exact AI workflow triggers, actions, provider and approval boundary are unspecified. | High | N/A | Select one initial AI use case and complete the AI decision checklist covering inputs, outputs, provider, data boundary, human approval, auditability and acceptance criteria. | AI lead | Sprint 0 | Open |
| I-04 | Issue | The planned repository walkthrough could not proceed because the client was unavailable, and the team currently does not have access to the starter repository. | High | N/A | Request repository access, propose a new walkthrough date and establish a deadline for activating the clean-slate fallback. Continue Sprint 0 work that does not depend on inherited code. | Repo steward | Immediate and weekly until resolved | Blocked |
| I-05 | Issue | The team does not currently have permission to create or manage a GitHub Project in the official repository. | Medium | N/A | Use a temporary team-member-owned repository for draft documentation, the GitHub Project board and task tracking. Ask Lecturer Leon or the repository administrator to resolve permissions. Migrate approved planning records after access is granted. | Repo steward | Next teaching-team contact | Blocked |
| I-06 | Issue | The MVP boundary and target business context have not yet been formally approved. | High | N/A | Prepare a concise scope proposal covering target users, core records, primary workflows, extensions and exclusions, and submit it to the Product Owner for approval. | Business analyst | Sprint 0 | Open |
| I-07 | Issue | The current user roles and record-access rules have not been defined. | High | N/A | Draft a role-permission matrix covering administrators, managers, sales representatives and read-only users, then request Product Owner confirmation. | Security lead | Before API authorisation work | Open |

## Dependencies

| ID | Type | Description | Impact | Likelihood | Response / next action | Owner | Review point | Status |
|---|---|---|---|---|---|---|---|---|
| D-01 | Dependency | Access to Peter Harding’s public Bootstrap repository and completion of the repository walkthrough. | High | N/A | Track through I-01 and I-04. Record the repository URL, licence, default branch and walkthrough date once confirmed. | Repo steward | Weekly until available | Blocked |
| D-02 | Dependency | Product Owner decisions regarding the target context, MVP boundary and first embedded AI workflow. | High | N/A | Maintain a prioritised open-question register and request written confirmation of each decision. Track unresolved scope through I-03 and I-06. | Business analyst | Sprint 0 | Pending |
| D-03 | Dependency | GitHub administrator permission to create or manage the official GitHub Project and related planning resources. | Medium | N/A | Continue using the documented temporary workaround and follow up with Lecturer Leon or the repository administrator. Track through I-05. | Repo steward | Next teaching-team contact | Blocked |
| D-04 | Dependency | Confirmation of the approved AI provider, API access and data-handling constraints. | High | N/A | Compare approved provider options, document security and privacy constraints, and avoid integrating production CRM data until approval is recorded. | AI lead | Before AI integration | Pending |
| D-05 | Dependency | Availability of the agreed deployment platform, database service and required environment credentials. | High | N/A | Confirm the deployment target, nominate a credential owner, document environment variables and test an early deployment using synthetic data. | DevOps lead | First integration milestone | Pending |

## Review procedure

At each RAID review, the team should:

1. Check whether any open risk has materialised and create or update the corresponding issue.
2. Confirm, invalidate or revise outstanding assumptions.
3. Update blocked issues with the latest follow-up action and review date.
4. Check whether external dependencies have become available.
5. Reassess impact and likelihood when new evidence is available.
6. Assign one accountable owner to every active entry.
7. Preserve closed entries as project history rather than deleting them.
8. Record important decisions in the decision log or an Architecture Decision Record where appropriate.

## Immediate priorities

The current highest-priority actions are:

1. Obtain access to the starter repository and confirm its licence.
2. Reschedule the client repository walkthrough.
3. Confirm the Product Owner and final acceptance authority.
4. Approve the MVP boundary and target business context.
5. Select and approve the first embedded AI workflow.
6. Confirm Sprint dates, milestones and the final delivery date.
7. Define the initial user roles and permission model.
8. Establish an early end-to-end integration and deployment path.
