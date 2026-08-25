# Core Domain Model

**Status:** Draft business model; not a final database schema

```mermaid
flowchart LR
    A[Account] -->|has or groups| C[Contact]
    A -->|has| O[Opportunity]
    L[Lead] -. may reference existing .-> A
    L -. conversion/linking pending .-> C
    L -. conversion/linking pending .-> O

    T[Task] -. relationship model pending .-> R[Approved CRM Record]
    E[Event] -. relationship model pending .-> R
    N[Interaction Note] -. relationship model pending .-> R
    R --- A
    R --- C
    R --- L
    R --- O

    T --> H[Activity History View]
    E --> H
    N --> H
```

## Confirmed domain meaning

- **Account:** an organisation or entity; not a bank account.
- **Contact:** a person, normally linked to an Account but potentially standalone.
- **Lead:** an early prospect that may refer to a new organisation or an existing Account.
- **Opportunity:** a specific potential sale with a stage and expected close date.
- **Task/Event:** follow-up or scheduled activities linked to CRM context.
- **Activity history:** a chronological view of interactions; it is not assumed to be a single database table.

## Design points still open

| Area | Decision required |
|---|---|
| Activities | One polymorphic relationship or entity-specific links. |
| Lead conversion | Records created/linked and transaction/rollback behaviour. |
| History | Which edits, notes and completed/cancelled activities remain visible. |
| Deletion | Hard delete versus archive/deactivate. |
| Extensions | Quotes, documents, users/roles and AI workflow records are outside the six-entity baseline until prioritised. |

Detailed fields and business rules remain in [requirements-and-scope.md](../product/requirements-and-scope.md).
