# Source Traceability Matrix

This matrix points to the supplied source-line ranges used to derive the initial backlog. Line references are to the original uploaded text files, not this generated pack.

| Trace ID | Source-derived statement | Source | Affected artefacts |
| --- | --- | --- | --- |
| TR-01 | AI-enabled CRM integrating with agents for workflow setup/implementation. | Project background lines 1-2 | Project vision; AI-01 to AI-06 |
| TR-02 | Initial schemas: accounts, contacts, leads, opportunities, tasks and events. | Project background line 4 | DISC-04; core epics |
| TR-03 | Research current CRMs, identify common features and compare with starter. | Transcript 51-71; 823-829 | DISC-01; Sprint 0 |
| TR-04 | Accounts are organisations/entities; contacts are people; sole traders may blur distinction. | Transcript 625-642 | ACC-01; CON-01; CON-02 |
| TR-05 | Lead may be new organisation or existing account and progresses through qualification. | Transcript 79-125 | LEAD-01 to LEAD-04 |
| TR-06 | Opportunity is a specific potential sale; close date is expected order/closure date. | Transcript 95-125 | OPP-01 to OPP-03 |
| TR-07 | Tasks/events are linked activities; interaction notes/history should be retained. | Transcript 126-180 | ACT-01 to ACT-05 |
| TR-08 | Current app has placeholders, holes, missing history and incomplete functions. | Transcript 29-45; 142-208 | DISC-02; risk R-03 |
| TR-09 | Real CRM needs users, authentication and roles. | Transcript 192-208 | SEC-01 to SEC-03 |
| TR-10 | AI may support team coordination and be integrated into the CRM product. | Transcript 392-430 | DEL-01; AI epic; Q-11/Q-12 |
| TR-11 | Start with Peter’s code, but team may choose another implementation; several stacks discussed. | Transcript 431-450; 745-757 | DEL-04; ADR-0001 |
| TR-12 | Public Bootstrap repo intended to remove Salesforce IP/look-and-feel. | Transcript 1-55; 456-473 | DISC-02; D-004 |
| TR-13 | Service example needs location-aware scheduling, duration, notifications and job knowledge. | Transcript 270-298 | ACT-06; AI-08; reference personas |
| TR-14 | Leon requested documented requirements/user stories and CRM research before implementation. | Transcript 711-829 | Entire kickoff pack |
| TR-15 | Slack preferred for shared client communication history. | Transcript 845-865 | Working agreement; action A-04 |

## Interpretation policy

- Where the transcript is unclear, the pack records a question or evidence status rather than silently repairing the meaning.
- Engineering safeguards such as synthetic data, CI, audit logging and human approval are labelled **Proposed** when not explicitly stated.
- The project background is treated as authoritative for the project title, initial schemas and client contact details.
