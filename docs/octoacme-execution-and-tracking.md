# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

### Role-Specific Daily Responsibilities
- **Developers**: update story status on the board, review and address PR comments, surface blockers in standup
- **QA**: move verified stories to Done, log new defects with severity and steps to reproduce, update test status
- **UX Designer**: provide async feedback on implementation PRs, update design files to reflect accepted changes
- **DevOps Engineer**: monitor pipeline health, respond to failed builds or deployments, update environment status
- **Data Analyst**: monitor key metric dashboards for anomalies, flag unexpected signals to PM
- **Project Manager**: update risk register, unblock dependencies, communicate status to stakeholders

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing

### QA Workflow
1. **Sprint planning**: QA reviews acceptance criteria and flags missing or ambiguous conditions before work begins.
2. **In development**: QA creates test plans and automated test cases in parallel with development.
3. **QA column**: Once a PR is merged, the story moves to the QA column. QA performs:
   - Functional testing against acceptance criteria
   - Regression testing of affected areas
   - Exploratory testing for edge cases
4. **Defect management**: Defects are logged with severity and steps to reproduce. Critical and high-severity defects block acceptance.
5. **Acceptance sign-off**: QA marks the story as accepted when all acceptance criteria pass and no open critical/high bugs remain.
6. **Release sign-off**: QA performs a final smoke test on the release candidate in the staging environment before production deployment.

### Acceptance Criteria by Role
| Role | Acceptance Standard |
|---|---|
| QA | All acceptance criteria verified; no open critical or high defects |
| Developers | Code reviewed and merged; unit and integration tests passing |
| UX Designer | Implementation matches approved design specs; accessibility requirements met |
| DevOps Engineer | Deployment pipeline passes; rollback procedure validated |
| Product Manager | Feature delivers agreed outcomes; demo accepted in sprint review |

### Quality Metrics
- **Defect escape rate**: defects found in production vs. defects found in QA (target: <10% escape rate)
- **Test coverage**: percentage of acceptance criteria covered by automated tests
- **Mean time to resolve defect**: average time from defect logged to verified fix
- **Regression pass rate**: percentage of regression suite passing per release candidate

- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

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
