# Open Product-Owner and Project Questions

Questions are ordered approximately by their effect on scope and delivery. Record answers in the decision log and update affected stories.

| ID | Area | Question | Why it matters |
| --- | --- | --- | --- |
| Q-01 | Governance | Who is the Product Owner and who gives final story/release acceptance: Peter, Peter and William jointly, or another arrangement? | Blocks backlog ordering and acceptance. |
| Q-02 | Product | Is the product a generic sales CRM, a service-business CRM, or a generic core demonstrated through a specific business such as organ maintenance or piano sales? | Determines fields, workflows and demo narrative. |
| Q-03 | Delivery | What are the sprint duration, client-review cadence, course milestones and final demonstration date? | Required for release planning and scope control. |
| Q-04 | Repository | What is the authoritative starter repository URL, branch, licence and access process? | Blocks code audit. |
| Q-05 | Architecture | What is the actual current stack in the public repo, and which parts are expected to be reused? | Transcript references FastAPI, Flask/server-side templates, Bootstrap and embedded React. |
| Q-06 | Architecture | Is React and/or Go a course learning objective, a client preference, or merely an option? | Prevents architecture novelty from overriding delivery. |
| Q-07 | Data | What exact fields are required for each initial entity, and which legacy fields should be removed? | Required for schema and forms. |
| Q-08 | Leads | What are the lead statuses, qualification criteria, disqualification reasons and conversion behaviour? | Required for lead workflow. |
| Q-09 | Opportunities | What stages, probability/amount fields and close rules are required? | Required for pipeline workflow. |
| Q-10 | Activities | Which records can tasks/events/notes relate to, and should activities use one polymorphic relationship or entity-specific links? | Affects schema and UI. |
| Q-11 | AI | What is the first product-facing AI workflow: summary, follow-up generation, natural-language workflow setup, notification drafting, route planning, or another use case? | Critical MVP decision. |
| Q-12 | AI | What does “set-up and implementation of workflows” mean in the expected demonstration: no-code configuration, natural-language drafting, execution, or all three? | Defines the central project feature. |
| Q-13 | AI | Which AI provider/model may be used, what data may be sent, and what retention/privacy constraints apply? | Required before connecting CRM data. |
| Q-14 | AI | Which actions may execute automatically, and which always require human approval? | Defines safety and acceptance tests. |
| Q-15 | Security | Is authentication/RBAC required in the first demonstrable increment or only before deployment? | Affects Sprint 1/2 ordering. |
| Q-16 | Security | Is the product single-organisation or multi-tenant, and what initial roles are needed? | Affects data model and authorisation. |
| Q-17 | Extensions | Are quotes part of the MVP despite not appearing in the six-schema project brief? | Controls scope. |
| Q-18 | Extensions | Are document attachments, reports/export and email notifications required? | Controls infrastructure and privacy work. |
| Q-19 | Reference vertical | Is route optimisation a core deliverable, a stretch demonstration or only an illustrative example? | Avoids accidental optimisation-project scope. |
| Q-20 | Data | Must the project import any existing CRM/Salesforce data, or will synthetic data be sufficient? | Affects migration, privacy and schedule. |
| Q-21 | Quality | What browsers, devices, hosting environment and availability expectations must be supported? | Defines non-functional acceptance. |
| Q-22 | Communication | Who should be in the Slack channel and what is the agreed weekly update/review time? | Reduces communication risk. |
