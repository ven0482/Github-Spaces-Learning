# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA / Testing

### Role Summary
QA Engineers validate that features meet acceptance criteria and quality standards before release. They design test plans, execute manual and automated tests, and act as the final quality gate.

### Responsibilities
- Define and maintain test plans and acceptance criteria
- Execute functional, regression, and exploratory testing
- Report, triage, and track defects to resolution
- Collaborate with developers on test automation strategies
- Verify fixes and perform release sign-off

### Quality Standards
- All critical and high-severity defects resolved before release
- Acceptance criteria verified for each user story
- Regression suite passing on the target environment
- Exploratory testing completed for new or changed flows

### Goals
- Prevent defects from reaching production
- Enable fast, confident releases through automation
- Maintain clear visibility into quality status for the team

### Typical Communication
- Participates in sprint planning to review acceptance criteria
- Daily standup: status of QA column items, blockers
- Bug reports and test summary reports in the project tracker

---

## UX Designer

### Role Summary
UX Designers create user experiences that are intuitive, accessible, and aligned with customer needs. They work closely with Product Managers and Developers to translate requirements into designs and validate usability.

### Responsibilities
- Conduct user research and synthesize insights
- Create wireframes, prototypes, and design specifications
- Define and maintain design system components
- Collaborate with developers during implementation to ensure fidelity
- Run usability tests and incorporate feedback into iterations

### Goals
- Deliver user experiences that meet customer needs and accessibility standards
- Reduce rework by involving design early in the feature lifecycle
- Maintain consistency across the product through shared design patterns

### Typical Communication
- Design reviews with Product Manager and developers before implementation begins
- Async design feedback via comments on design files or PRs
- Usability test readouts shared with the full team

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the infrastructure, CI/CD pipelines, and release processes that enable the team to ship reliably and safely. They act as a bridge between development and operations.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines
- Manage cloud infrastructure, environments, and configuration
- Implement monitoring, alerting, and observability tooling
- Coordinate and execute production deployments and rollbacks
- Enforce security and compliance controls in the delivery pipeline

### Goals
- Enable fast, reliable, and repeatable deployments
- Reduce mean time to recovery (MTTR) for production incidents
- Maintain infrastructure as code for consistency and auditability

### Typical Communication
- Release planning meetings with PM and developers
- Incident retrospectives and post-mortem write-ups
- Infrastructure change notifications shared with the delivery team

---

## Data Analyst

### Role Summary
Data Analysts measure product outcomes, monitor key metrics, and surface insights that inform prioritization and decision-making across the team.

### Responsibilities
- Define and track success metrics for features and releases
- Build and maintain dashboards and reports for the delivery team
- Analyze usage data to identify trends, anomalies, and opportunities
- Collaborate with Product Managers on experiment design and results
- Provide data to support go/no-go release decisions

### Goals
- Ensure the team has timely, accurate data to make evidence-based decisions
- Close the feedback loop between releases and measurable outcomes
- Surface early signals of quality or adoption issues post-release

### Typical Communication
- Weekly metric reviews with Product Manager and Project Manager
- Post-release analysis shared with the full team
- Ad-hoc data pulls in response to stakeholder or team questions

---

## Stakeholders

### Role Summary
Stakeholders are individuals or groups with a vested interest in the project's outcomes. They provide strategic direction, approve key decisions, and represent customer or business priorities.

### Stakeholder Types
- **Executive Sponsors**: Provide budget approval, strategic alignment, and escalation support
- **Business Owners**: Define business requirements and validate that outcomes meet organizational goals
- **End Users / Customers**: Use the product and provide feedback on usability and value
- **Regulatory / Compliance**: Review deliverables for legal, security, or compliance requirements
- **Partner Teams**: Depend on or integrate with the project's outputs

### Responsibilities
- Provide timely input on requirements and priorities
- Review and approve key project milestones and deliverables
- Escalate issues or unblock decisions within their area of authority
- Attend stakeholder briefings and provide actionable feedback

### Goals
- Ensure the project delivers value to their area of the business or customer base
- Maintain visibility into progress, risks, and changes

### Typical Communication
- Monthly stakeholder updates from the Project Manager
- Ad-hoc briefings for major scope changes or escalations
- Approval checkpoints at initiation, planning, and release stages

---

## Role Interaction Matrix

This matrix summarizes the key collaboration touchpoints between roles during each project phase.

| Phase | Roles Involved | Key Interaction |
|---|---|---|
| Initiation | Project Manager, Product Manager, Stakeholders | Align on problem statement, success metrics, and scope |
| Planning | Project Manager, Product Manager, Developers, UX Designer | Break down backlog, define acceptance criteria, estimate effort |
| Design | UX Designer, Product Manager, Developers | Design reviews; handoff of specs and prototypes |
| Development | Developers, QA, UX Designer, DevOps Engineer | Implementation, code review, test automation, environment setup |
| QA & Testing | QA, Developers, Product Manager | Test execution, defect triage, acceptance sign-off |
| Release | DevOps Engineer, QA, Project Manager, Product Manager | Deployment coordination, release sign-off, rollback planning |
| Post-Release | Data Analyst, Product Manager, Project Manager, Stakeholders | Metric review, outcome validation, lessons learned |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

