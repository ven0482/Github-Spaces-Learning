# OctoAcme — Roles Interaction Matrix

## Purpose
Document when and how roles collaborate across the project lifecycle, clarify handoff points, and reduce confusion about role boundaries and dependencies.

---

## Interaction Patterns by Phase

### 1. Initiation

| Interaction | Roles Involved | Description |
|---|---|---|
| Problem statement alignment | Project Manager, Product Manager, Executive Sponsors | PM and PdM draft the project one-pager; sponsors review and approve scope and success criteria |
| Stakeholder identification | Project Manager, Product Manager | Identify all stakeholder types (executive, business owner, end user, partner team) and assign communication owners |
| Initial risk assessment | Project Manager, Developers (lead), DevOps Engineer | Surface known technical, infrastructure, and schedule risks before planning begins |

---

### 2. Planning

| Interaction | Roles Involved | Description |
|---|---|---|
| Backlog refinement | Product Manager, Developers, QA, UX Designer | PdM presents prioritized stories; UX Designer shares research inputs; Developers and QA raise questions and flag missing acceptance criteria |
| Effort estimation | Developers, QA, DevOps Engineer | Estimate development, testing, and infrastructure work; surface dependencies between items |
| Design handoff preparation | UX Designer, Product Manager | UX Designer presents wireframes and prototypes for upcoming sprint; PdM confirms alignment with requirements |
| Release planning | Project Manager, DevOps Engineer, QA | Agree on release schedule, environment availability, and QA sign-off milestones |

---

### 3. Design

| Interaction | Roles Involved | Description |
|---|---|---|
| Design review | UX Designer, Product Manager, Developers | UX Designer presents final designs; Developers raise implementation questions; PdM confirms requirements coverage |
| Accessibility and standards check | UX Designer, QA | UX Designer documents accessibility requirements; QA adds accessibility checks to the test plan |
| Design spec handoff | UX Designer, Developers | UX Designer delivers annotated specs and assets; Developers confirm they have sufficient detail to begin implementation |

---

### 4. Development

| Interaction | Roles Involved | Description |
|---|---|---|
| Implementation support | Developers, UX Designer | Developers raise design questions in PR comments or async channels; UX Designer responds within agreed SLA (e.g., same business day) |
| Test automation collaboration | Developers, QA | Developers and QA agree on what to automate vs. test manually; QA reviews test coverage in PRs |
| Infrastructure and environment readiness | Developers, DevOps Engineer | DevOps Engineer ensures environments are ready; Developers flag any infrastructure dependencies as stories are picked up |
| Code review | Developers | Peer code review; PRs require at least one approval before merging |

---

### 5. QA & Testing

| Interaction | Roles Involved | Description |
|---|---|---|
| Test execution and defect logging | QA, Developers | QA logs defects with steps to reproduce and severity; Developers prioritize and fix defects; QA verifies fixes |
| Acceptance sign-off | QA, Product Manager | QA confirms acceptance criteria are met; PdM reviews the feature in a demo or async walkthrough before marking the story Done |
| Design fidelity check | QA, UX Designer | QA flags visual or interaction deviations from design specs; UX Designer reviews and confirms acceptable tolerances |
| Performance and security validation | QA, DevOps Engineer | QA includes performance and security checks in the test plan; DevOps Engineer provides scan results and benchmark data |

---

### 6. Release

| Interaction | Roles Involved | Description |
|---|---|---|
| Release readiness review | Project Manager, QA, DevOps Engineer, Product Manager | Team confirms all stories are accepted, no blocking defects remain, and the deployment plan is ready |
| Production deployment | DevOps Engineer, QA, Project Manager | DevOps Engineer executes the deployment; QA runs post-deployment smoke tests; PM monitors for issues |
| Rollback decision | DevOps Engineer, Project Manager, Product Manager | If critical issues are found, PM and PdM make the go/no-go rollback decision; DevOps Engineer executes |
| Release announcement | Project Manager, Product Manager, Stakeholders | PM communicates release notes and outcomes to stakeholders |

---

### 7. Post-Release

| Interaction | Roles Involved | Description |
|---|---|---|
| Metric review | Data Analyst, Product Manager, Project Manager | Data Analyst presents post-release metrics; team evaluates against success criteria defined in the project one-pager |
| Stakeholder outcome briefing | Project Manager, Product Manager, Executive Sponsors | PM summarizes delivery outcomes, lessons learned, and next steps |
| Retrospective | Full delivery team | Team reflects on what went well, what to improve, and captures action items |
| Backlog updates from data | Data Analyst, Product Manager | Data Analyst surfaces opportunities or issues from post-release data; PdM incorporates insights into the roadmap |

---

## Common Role Handoffs

### Feature from Design to Development
1. UX Designer completes and reviews design with Product Manager.
2. UX Designer publishes annotated spec and assets to the shared design tool.
3. Product Manager updates the story with a link to the design spec.
4. Developer picks up the story, confirms all assets are available, and tags UX Designer if questions arise.

### Story from Development to QA
1. Developer merges the PR and moves the story to the QA column.
2. QA picks up the story, reviews acceptance criteria, and begins test execution.
3. QA logs any defects and assigns them to the developer.
4. Developer fixes defects; QA verifies and either accepts the story or logs further issues.

### Release from QA to DevOps
1. QA completes final smoke test on the staging environment and confirms release sign-off.
2. QA documents the sign-off in the project tracker (e.g., closes the QA checklist issue).
3. DevOps Engineer receives the green light and executes the production deployment.
4. QA performs post-deployment verification; DevOps Engineer monitors infrastructure metrics.

---

## Escalation Paths

| Situation | Escalation Path |
|---|---|
| Defect blocks release | QA → Project Manager → Product Manager (go/no-go decision) |
| Design disagreement during implementation | Developer → UX Designer → Product Manager (final decision) |
| Infrastructure outage or deployment failure | DevOps Engineer → Project Manager → Executive Sponsor if customer-impacting |
| Metric anomaly post-release | Data Analyst → Product Manager → Project Manager |
| Scope change request | Stakeholder → Product Manager → Project Manager (impact assessment and approval) |
