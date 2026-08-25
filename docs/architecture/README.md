# Architecture Documentation

**Current phase:** Discovery. The client starter repository and walkthrough are still pending, so these documents describe an evidence-based baseline and decision process, not a verified as-built system.

| Document | Purpose |
|---|---|
| [architecture-overview.md](architecture-overview.md) | Known technical evidence, logical boundaries and unresolved architecture points. |
| [domain-model.md](domain-model.md) | Technology-neutral CRM entities, relationships and open data-design questions. |
| [starter-repository-audit.md](starter-repository-audit.md) | Evidence to collect when repository access is available. |
| [adr-0001-architecture-selection.md](adr-0001-architecture-selection.md) | Records the application architecture options and eventual decision. |

## Maintenance rules

- Do not describe transcript claims as verified implementation facts until the code is inspected.
- Use the overview for the current architecture picture; use ADRs for decisions and trade-offs.
- Keep the domain model independent of framework and database-table details.
- Add API, deployment and security design documents only after the architecture is selected or those areas enter active delivery.
