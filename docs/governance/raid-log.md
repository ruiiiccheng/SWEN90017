# RAID Log

**Scale:** Impact and likelihood are qualitative initial assessments for refinement.

| ID | Type | Description | Impact | Likelihood | Response / next action | Owner | Status |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R-01 | Risk | MVP and target vertical remain ambiguous. | High | High | Confirm with Product Owner in Sprint 0; maintain explicit in/out/later scope. | Product Owner + Scrum Master | Open |
| R-02 | Risk | Starter repository may be delayed, incomplete or difficult to run. | High | Medium | Request access immediately; time-box audit once access is granted; continue non-dependent Sprint 0 work; keep a clean-slate fallback. | Technical lead | Materialised — see I-04 |
| R-03 | Risk | Inherited screens may look complete but contain placeholders or broken links. | High | High | Capability audit and automated end-to-end smoke tests before planning reuse. | Development team | Open |
| R-04 | Risk | Salesforce branding/look-and-feel may create IP concerns. | High | Medium | Use public Bootstrap version; remove copied assets and avoid design cloning. | Repo steward | Open |
| R-05 | Risk | A full React/Go rewrite could consume the schedule before user value is delivered. | High | Medium | Architecture spike with explicit delivery-risk criterion and vertical-slice proof. | Technical team | Open |
| R-06 | Risk | “AI-enabled” may be interpreted as team-agent coordination rather than a product feature, or vice versa. | High | High | Separate both tracks and obtain Product Owner approval for the first embedded use case. | Product Owner + AI lead | Open |
| R-07 | Risk | AI processing could expose personal or commercially sensitive CRM data. | High | Medium | Synthetic data; approved provider/policy; minimum context; human approval and audit. | Security/AI lead | Open |
| R-08 | Risk | Communication is fragmented across WeChat, Slack, email and GitHub. | Medium | High | Define Slack/GitHub as durable source; copy decisions from informal chat. | Scrum Master | Open |
| R-09 | Risk | Team skill gaps in Go, React or inherited Python stack may reduce velocity. | Medium | Medium | Skills inventory, pairing, spike and architecture decision based on evidence. | Technical team | Open |
| R-10 | Risk | Route optimisation can become a separate complex optimisation product. | High | Medium | Keep it as an optional constrained pilot unless explicitly prioritised. | Product Owner | Open |
| R-11 | Risk | Legacy data model may contain unnecessary fields and relationships. | Medium | High | Create a simplified data dictionary and migrate only approved fields. | Data lead | Open |
| R-12 | Risk | Meeting transcript contains recognition and speaker-attribution errors. | Medium | High | Validate open questions; tag requirements by evidence; do not treat uncertain wording as fact. | Business analyst | Open |
| A-01 | Assumption | Peter is the primary Product Owner and final acceptance authority. | High | N/A | Confirm explicitly. | Student team | Unconfirmed |
| A-02 | Assumption | Synthetic data can be used for all development and demonstrations. | High | N/A | Confirm data expectations and import requirements. | Student team | Unconfirmed |
| A-03 | Assumption | The initial MVP can focus on a sales CRM core even if demonstrated through a service business. | High | N/A | Confirm target context. | Product Owner | Unconfirmed |
| I-01 | Issue | Exact repository URL, licence and current branch are not present in the transcript. | High | N/A | Obtain access and record repository metadata. | Repo steward | Open |
| I-02 | Issue | Sprint duration, milestones and final delivery date are not documented. | High | N/A | Align with course calendar and client availability. | Scrum Master | Open |
| I-03 | Issue | Exact workflow triggers/actions and AI provider are unspecified. | High | N/A | Select one use case and complete AI decision checklist. | AI lead + Product Owner | Open |
| I-04 | Issue | Planned repository walkthrough could not proceed because the client was unavailable, and the team currently does not have access to the client starter repository. | High | N/A | Request repository access and reschedule the walkthrough; continue Sprint 0 work that does not depend on the inherited codebase; keep related documentation current. | Scrum Master / Repo steward | Blocked |
| I-05 | Issue | The team does not currently have permission to create or manage a GitHub Project in the official repository. | Medium | N/A | Use a temporary team-member-owned repository for draft documentation, the GitHub Project board and task tracking; ask Lecturer Leon / the repository administrator to resolve permissions next week; migrate the temporary planning records back to the official repository once access is available. | Scrum Master / Repo steward | Blocked — workaround active |
| D-01 | Dependency | Peter’s public Bootstrap repository and walkthrough. | High | N/A | Track action A-01/A-02. | Peter Harding | Open |
| D-02 | Dependency | Product-owner answers to target context, MVP and AI workflow. | High | N/A | Review open-question register. | Product Owner | Open |
