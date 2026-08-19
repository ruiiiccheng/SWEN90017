# Definition of Ready and Definition of Done

## Definition of Ready

A story may enter a sprint when:

- The user/persona, need and value are clear.
- Acceptance criteria are testable and understood by the team.
- Evidence status is known: confirmed, proposed or decision pending.
- Required fields, relationships and lifecycle rules are defined or explicitly constrained for the sprint.
- Dependencies and external decisions are resolved or have an agreed fallback.
- UI/API/data/security implications have been considered.
- AI stories state authorised context, expected structured output, uncertainty behaviour, human-approval boundary and audit behaviour.
- Test data is available or can be created safely.
- The team has estimated the story and believes it fits within the sprint.

## Definition of Done

A story is done when:

- Every acceptance criterion passes and the Product Owner can demonstrate the intended outcome.
- Code is merged through a reviewed pull request; no direct unreviewed change is made to main.
- Automated tests cover the important success and failure paths at the appropriate level.
- Database/schema changes include a tested migration and rollback/forward strategy appropriate to the project.
- Validation and error states are usable and do not expose sensitive implementation details.
- Authentication/authorisation checks are server-side where the story requires them.
- AI behaviour is bounded to supported actions, records relevant provenance/context, and follows the approved human-control/data policy.
- Documentation, source trace and decision records are updated.
- The feature works with the agreed synthetic dataset and supported viewport/browser baseline.
- No Salesforce branding, copied interface asset or secret is introduced.
- CI passes and no known critical defect remains in the delivered scenario.
- The team demonstrates the story in Sprint Review and the Product Owner accepts it or records specific follow-up work.

## Bug severity guide

| Severity | Meaning | Expected handling |
|---|---|---|
| Critical | Security/privacy breach, data loss/corruption, or system cannot start | Stop release/sprint goal and address immediately |
| High | Core accepted workflow cannot complete and no reasonable workaround exists | Fix before story/release acceptance |
| Medium | Material defect with a workaround or limited scope | Prioritise in current/next sprint |
| Low | Cosmetic or minor usability issue | Backlog and prioritise normally |
