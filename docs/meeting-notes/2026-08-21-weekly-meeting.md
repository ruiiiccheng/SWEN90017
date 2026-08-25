# Weekly Team Meeting — Sprint 1 Blocker and Preparation

**Date/time:** 25 August 2026  
**Attendees:** Team 6 
**Facilitator:** TBD  
**Note taker:** TBD

## Objectives

- Review current Sprint 1 progress and identify blockers, including repository access and GitHub Project permissions.
- Agree on productive work that can continue while access to the client starter repository is pending.
- Prepare useful material for the next client discussion with Peter.

## Demonstrated work

- Reviewed the current project documentation and Sprint 1 plan.
- Reviewed the dependency on the client repository and planned repository walkthrough.
- Confirmed that the team currently cannot create or manage a GitHub Project in the official repository.

## Discussion and clarifications

- The team recognised that the planned repository walkthrough could not proceed because the client was unavailable.
- The team currently does not have access to the client starter repository. This blocks the starter-code audit and prevents the team from independently verifying the inherited implementation, exact technology stack, setup process, and reusable components.
- The team agreed that this blocker should be explicitly tracked rather than allowing it to stall all Sprint 1 work.
- The team also identified a second blocker: current permissions on the official repository do not allow the team to create or manage the GitHub Project used for Sprint planning and task tracking.
- As a temporary workaround, a team member will provide a separate repository where the team can maintain draft documentation, a GitHub Project board and tasks. This temporary repository is a staging/coordination workspace rather than the final source of truth.
- The team plans to ask Lecturer Leon / the repository administrator to resolve the official repository permissions when Leon returns next week. Once permissions are restored, the temporary planning records should be migrated back to the official repository.
- Work that does not depend on the inherited repository can continue, including requirements refinement, documentation maintenance, product and workflow clarification, and interface exploration.
- The team agreed to prepare a low-fidelity prototype to make the next discussion with Peter more concrete and to obtain early feedback on the intended CRM workflow and interface direction.

## Decisions

| ID | Decision | Owner | Date | Affected stories/docs |
|---|---|---|---|---|
| WM-01 | Formally track the missing repository access and postponed walkthrough as a current blocker in the RAID log. | Scrum Master / Repo steward | 2026-08-25 | `docs/governance/raid-log.md`, DISC-02 |
| WM-02 | Continue Sprint 1 work that is not dependent on access to the inherited codebase. | Whole team | 2026-08-25 | Sprint 1 backlog |
| WM-03 | Review and update the current project documentation so requirements, assumptions, open questions, risks and Sprint status remain consistent with the team's latest understanding. | Whole team | 2026-08-25 | `docs/`, `backlog/` |
| WM-04 | Create a low-fidelity prototype for the agreed core CRM flow and use it as a discussion artefact in the next review with Peter. | Whole team | 2026-08-25 | Product/workflow design, Sprint 1 review |
| WM-05 | Temporarily use a team-member-owned repository for draft docs, the GitHub Project board and task tracking while GitHub Project permissions are unavailable in the official repository. The official repository remains the intended final source of truth. | Whole team | 2026-08-25 | GitHub Project, task tracking, `docs/` |

## Actions

| ID | Owner | Action | Due | Status |
|---|---|---|---|---|
| WA-01 | Scrum Master / Repo steward | Request or follow up on access to the client starter repository and arrange a repository walkthrough with Peter. | Before next client meeting | Pending |
| WA-02 | Whole team | Review and update existing project documents to reflect current knowledge, assumptions, open questions and blockers. | Before next client meeting | In progress |
| WA-03 | Design / development team | Produce a low-fidelity prototype of the core CRM workflow for discussion with Peter. | Before next client meeting | Planned |
| WA-04 | Technical team | Begin the starter-code audit as soon as repository access is available; avoid finalising architecture assumptions before inspecting the inherited codebase. | After repository access | Blocked |
| WA-05 | Scrum Master / Repo steward | Ask Lecturer Leon / the repository administrator to enable the required GitHub Project permissions in the official repository. | Next week, when Leon returns | Pending |
| WA-06 | Scrum Master / Repo steward | After official permissions are restored, migrate or recreate the temporary GitHub Project items, tasks and approved documentation changes in the official repository and confirm one source of truth. | After permission issue is resolved | Planned |

## Risks/blockers

### Blocker 1 — Client starter repository access

- **Current blocker:** The team does not yet have access to the client starter repository, and the planned repository walkthrough has not been completed.
- **Impact:** DISC-02 (starter-code audit), inherited-system verification, environment setup based on the client codebase, and evidence-based architecture decisions are blocked or constrained.
- **Mitigation:** Continue non-dependent Sprint 1 tasks, keep project documentation current, and prepare a low-fi prototype so the next client session can still generate actionable feedback.

### Blocker 2 — GitHub Project permissions in the official repository

- **Current blocker:** The team cannot currently create or manage the GitHub Project used for planning and task tracking in the official repository.
- **Impact:** Sprint tasks and planning artefacts cannot yet be maintained in their intended official location.
- **Workaround:** Use a temporary team-member-owned repository for draft documentation, the GitHub Project board and tasks. Treat it as a temporary coordination workspace only.
- **Resolution:** Ask Lecturer Leon / the repository administrator to resolve permissions next week, then migrate the temporary planning records back to the official repository and re-establish a single source of truth.

## Questions requiring client answer

- What is the authoritative starter repository, branch and access method?
- What is the actual current technology stack in the repository, and which parts does Peter expect the team to reuse?
- Can Peter provide a repository walkthrough at the next client session?
- Does the proposed low-fi CRM workflow match the intended MVP and demonstration scenario?

## Next meeting

- **Date/time:** To be confirmed
- **Expected demonstration:** Low-fidelity prototype of the proposed core CRM workflow, together with updated project documentation and a concise list of repository/architecture questions for Peter. The team should also review the status of official GitHub Project permissions and the planned migration from the temporary workspace.
