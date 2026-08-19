# Sprint 1 Proposal — Connected Customer Record Vertical Slice

## Proposed sprint goal

Demonstrate that a user can create an account, add a linked contact, create a related follow-up activity, and see the connected context in one record view.

This goal is deliberately narrower than “implement the CRM”. It exercises data modelling, UI, API/server behaviour, lookups, relationships, migrations, validation and tests in one demonstrable slice.

## Candidate committed stories

- ACC-01 — Create and maintain accounts.
- CON-01 — Create and maintain contacts.
- CON-02 — Link contacts to accounts.
- ACC-02 — Search accounts and contacts.
- ACC-03 — View a connected customer record, limited initially to implemented relationships.
- ACT-01 — Create and maintain related tasks.

## Candidate stretch stories

- ACT-02 — Create and maintain related events.
- ACT-03 — Display a unified activity timeline.
- ACT-04 — Record interaction notes.

## Technical/enabler work included in the stories

- Database migrations and seed fixtures.
- API/server validation and error handling.
- Automated tests for the chosen acceptance scenarios.
- Responsive form/list/detail behaviour at agreed widths.
- Removal of any remaining Salesforce-specific presentation from touched pages.
- Documentation and demo script.

## Example acceptance scenario

1. Sign in or enter the approved local prototype mode.
2. Create “Example Service Company” as an account.
3. Create “Alex Example” as a contact and link the contact to that account using lookup.
4. Create a high-priority follow-up task due on a future date and link it to the account/contact.
5. Open the account and see the contact and open task in context.
6. Edit the contact, complete the task and verify the history remains available.

## Sprint review questions

- Does the relationship model match how the client thinks about accounts and contacts?
- Is lookup sufficiently clear to prevent linking the wrong record?
- Which fields are actually essential for the next lead/opportunity slice?
- Should authentication be brought forward before broader functionality?
- Is the activity presentation suitable for the selected reference business?
