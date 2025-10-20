# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
- **DevOps ownership**: DevOps Engineers own CI/CD pipeline configuration, deployment automation, and infrastructure reliability
- **UX and QA collaboration**: UX Designers collaborate with QA on accessibility and usability checks before release (see [Handoff Checklists](octoacme-handoff-checklists.md))

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (coordinated by Security Lead)
- Manual QA for feature acceptance when needed
- **Security Lead responsibilities**: Manage vulnerability scanning, conduct security reviews, and coordinate incident response paths

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Key handoffs planned using [Handoff Checklists](octoacme-handoff-checklists.md)
- [ ] Role assignments confirmed per [Role Interaction Matrix](octoacme-role-interaction-matrix.md)
- [ ] DevOps Engineer assigned for CI/CD and infrastructure
- [ ] Security Lead engaged for security reviews
- [ ] UX Designer and QA coordinating on accessibility validation
