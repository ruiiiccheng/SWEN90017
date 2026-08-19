# Decision Log

| ID | Decision | Basis | Rationale | Status |
| --- | --- | --- | --- | --- |
| D-001 | Use the supplied brief and transcript as a discovery baseline, not a final specification. | Confirmed process direction | Prevents uncertain transcript wording becoming an unreviewed requirement. | Accepted |
| D-002 | Begin with CRM research, requirements/user stories and a starter-code gap analysis before major implementation. | Confirmed | Repeated direction from Peter and Leon. | Accepted |
| D-003 | Initial domain baseline is accounts, contacts, leads, opportunities, tasks and events. | Confirmed | Explicit project background. | Accepted |
| D-004 | Do not deliver Salesforce branding or copied look-and-feel. | Confirmed | Client identified copyright/IP concern and is preparing a Bootstrap version. | Accepted |
| D-005 | Start by evaluating Peter’s starter code, while retaining the option to replace parts or all of it. | Confirmed | Client advised starting with his code but left final approach to the team. | Accepted |
| D-006 | Use GitHub and Markdown for durable planning/project memory; use Slack for client-visible history. | Confirmed | Meeting collaboration discussion. | Accepted |
| D-007 | Final application architecture is deferred to a time-boxed spike. | Decision pending | Python/server-rendered, React/Python API and React/Go API were all discussed. | Open |
| D-008 | The first embedded AI workflow is not yet selected. | Decision pending | Agent scope remained ambiguous. | Open |
| D-009 | Use human approval for consequential AI actions. | Proposed | Recommended safety/control baseline; requires Product Owner approval. | Proposed |
| D-010 | Use synthetic data unless real-data use is explicitly approved. | Proposed | Reduces privacy and confidentiality risk. | Proposed |

For architecture decisions with substantial trade-offs, create a dedicated ADR under `docs/architecture/` and link it here.
