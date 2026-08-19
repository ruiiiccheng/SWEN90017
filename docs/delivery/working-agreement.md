# Team Working Agreement

## Communication

- Use **Slack** for client-visible questions, decisions and weekly updates.
- WeChat may be used for fast internal discussion, but any material decision, requirement change or client question must be copied into Slack and/or the repository.
- Use a short weekly written update: completed, next, risks/blockers, decisions/questions needed.

## Source of truth

- Product backlog: `backlog/product-backlog.md` and the active GitHub Project/issue set.
- Decisions: `docs/governance/decision-log.md` and ADRs.
- Client answers: meeting notes plus linked Slack summary.
- Technical setup: repository README and architecture documents.
- Individual/agent context: member-memory files; not private chat alone.

## Git workflow

- Protect `main`; merge only reviewed pull requests.
- Suggested branch names: `feature/<story-id>-short-name`, `fix/<issue-id>-short-name`, `docs/<topic>`.
- One primary backlog item per pull request where practical.
- Pull requests link the story/issue, list acceptance criteria, tests and screenshots/evidence where relevant.
- Resolve review comments before merge or record why they are not applicable.

## Scrum ceremonies

- **Stand-up:** brief daily or class-day check-in: goal, progress, blocker, coordination need.
- **Refinement:** at least once per sprint; include the Product Owner for decisions that change meaning or priority.
- **Planning:** select a sprint goal first, then capacity-appropriate stories that meet Ready.
- **Review:** demonstrate working software against acceptance criteria; record accept/reject/follow-up.
- **Retrospective:** choose one or two process improvements with owners.

## AI-assisted development

- A team member remains accountable for every AI-generated change.
- Do not merge generated code without understanding, tests and review.
- Record important prompts/constraints or generated design decisions when they affect maintainability.
- Never paste real client secrets or personal data into an unapproved AI tool.
- Agents may propose changes; repository review and CI remain the control point.
