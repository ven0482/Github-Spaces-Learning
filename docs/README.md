# OctoAcme Project Management Docs

## Project Overview

This folder contains OctoAcme's project management process documentation. These documents define how the team initiates, plans, executes, releases, and retrospects on projects. They serve as the single source of truth for team workflows, role responsibilities, quality standards, and communication cadences. New team members should read these docs to quickly get up to speed, and the team should keep them updated as processes evolve.

## Process Summary

**Lifecycle & Planning Approach**
OctoAcme follows a five-phase project lifecycle: Initiation, Planning, Execution, Release, and Close & Retrospective. Work begins with a Project One-pager that captures the problem statement, SMART goal, success metrics, and key stakeholders. Before moving into planning, a decision gate confirms that success metrics are clear and team availability is secured. During planning, the team creates a prioritized backlog with acceptance criteria, defines the Definition of Done (DoD), estimates effort, and maps dependencies and milestones into a release plan.

**Execution & Delivery Workflows**
Day-to-day execution is driven by a regular team rhythm: daily 15-minute standups focused on progress and blockers, weekly delivery syncs to surface risks and updates, and end-of-sprint demos. Work moves through a standard project board with columns: Backlog, Ready, In Progress, In Review, QA, and Done. Pull requests are kept small (≤ 400 lines when possible), must link to the relevant issue and acceptance criteria, and require passing CI checks and at least one approval before merging. Quality assurance is embedded throughout — unit tests, integration tests, end-to-end smoke tests, and security scanning run in CI, with manual QA for feature acceptance as needed.

**Roles & Communication**
Three core personas drive OctoAcme projects. The **Project Manager (PM)** coordinates delivery, manages schedules, risks, and cross-team communication. The **Product Manager (PdM)** owns the product vision, defines problem statements, prioritizes the backlog, and measures outcomes. **Developers** implement features and fixes, write tests, and participate in design and code reviews. Communication flows through a weekly PM–PdM alignment sync, twice-weekly team standups, and monthly stakeholder updates. Blockers escalate through three levels: team-level triage in standup → PM escalation to the Product Lead and dependent teams → sponsor-level escalation for business-impacting issues.

**Continuous Improvement**
Risks are tracked in a Risk Register (ID, description, impact, likelihood, owner, mitigation, status) and reviewed at every weekly sync. After each sprint, release, or significant milestone the team holds a retrospective structured around what went well, what could be improved, and 2–3 prioritized action items with owners and due dates. Action items are added to the project backlog and reviewed in the weekly PM sync. Over time, measuring the impact of these improvements and celebrating wins reinforces a culture of iterative, data-informed process change.

## Document Index

| Document | Description |
|---|---|
| [octoacme-project-management-overview.md](octoacme-project-management-overview.md) | High-level summary of OctoAcme's project management principles, core roles, key artifacts, lifecycle phases, and communication cadence |
| [octoacme-project-initiation.md](octoacme-project-initiation.md) | Guide for validating and authorizing new work — covers the Project One-pager template, stakeholder alignment, and the initiation decision gate |
| [octoacme-project-planning.md](octoacme-project-planning.md) | How to turn an approved initiative into an actionable backlog — kickoff, estimation, Definition of Done, dependency mapping, and release planning |
| [octoacme-execution-and-tracking.md](octoacme-execution-and-tracking.md) | Day-to-day execution guidance — team rhythm, project board workflow, PR conventions, quality & testing standards, and blocker escalation |
| [octoacme-release-and-deployment.md](octoacme-release-and-deployment.md) | Standardized release process — release types, pre-release requirements, deployment checklist, rollback playbook, and release notes template |
| [octoacme-retrospective-and-continuous-improvement.md](octoacme-retrospective-and-continuous-improvement.md) | How to run post-sprint and post-release retrospectives, track action items, and build a continuous improvement culture |
| [octoacme-risks-and-communication.md](octoacme-risks-and-communication.md) | Risk register structure, risk lifecycle (identify → assess → mitigate → monitor), stakeholder communication templates, and escalation paths |
| [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) | Detailed role definitions for Project Managers, Product Managers, and Developers — responsibilities, goals, and typical communication patterns |

## Getting Started

If you are new to the team, here is the recommended reading order:

1. **Start with the overview** — read [octoacme-project-management-overview.md](octoacme-project-management-overview.md) to understand OctoAcme's guiding principles, lifecycle, and key artifacts.
2. **Know your role** — find your persona in [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) to understand your responsibilities and communication expectations.
3. **Follow the lifecycle** — work through the phase-specific guides in order: initiation → planning → execution → release → retrospective.
4. **Check the communication and risk docs** — [octoacme-risks-and-communication.md](octoacme-risks-and-communication.md) covers escalation paths and the templates you will use for weekly status updates.
5. **Bookmark the execution guide** — [octoacme-execution-and-tracking.md](octoacme-execution-and-tracking.md) is the reference you will return to most often during active delivery.

When starting a new project, create a Project One-pager using the template in the initiation guide, store it in the project repository, and add the relevant process docs to `.copilot/` if you want GitHub Copilot to use them as context.
