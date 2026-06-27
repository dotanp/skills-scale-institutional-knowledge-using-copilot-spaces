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

## QA / Test Engineers

### Role Summary
QA/Test Engineers own the quality strategy for a project. They validate that delivered work meets acceptance criteria and the Definition of Done, and champion testability throughout delivery.

### Responsibilities
- Define and maintain the test plan and QA approach
- Validate features against acceptance criteria and the Definition of Done
- Author and maintain integration and end-to-end smoke tests for critical flows
- Triage defects with Developers and confirm fixes
- Provide release-readiness and quality signals
- Run manual QA for feature acceptance when needed

### Goals
- Catch defects early and reduce escaped bugs
- Maintain high confidence in releases
- Improve test coverage and observability of quality

### Typical Communication
- Daily standups and bug triage
- Acceptance sign-off and release-readiness updates
- Test plans and QA notes

### How this role interacts with existing roles
- **Developers:** pairs on testability, reproduces and verifies defects
- **Product Managers:** confirms acceptance criteria and validates feature acceptance
- **Project Managers:** reports quality signals, risks, and release readiness

---

## Engineering Lead / Tech Lead

### Role Summary
Engineering Leads own technical direction, architecture decisions, and code-review standards for the delivery team.

### Responsibilities
- Set technical direction and architecture
- Uphold code-review and quality standards
- Identify and mitigate technical risks
- Coordinate cross-team technical dependencies and integration points
- Support estimation and breakdown of work
- Mentor Developers

### Goals
- Maintainable, scalable architecture
- Consistent engineering quality
- Reduced technical risk and rework

### Typical Communication
- Technical design docs and reviews
- Standups and planning
- Risk/trade-off discussions with Product and Project Managers

### How this role interacts with existing roles
- **Developers:** guides design and review, unblocks technical issues
- **Product Managers:** surfaces effort and feasibility trade-offs
- **Project Managers:** flags technical risks and cross-team dependencies

---

## Designers (UX/UI)

### Role Summary
Designers own the user experience, interaction design, and usability of features.

### Responsibilities
- Research and frame user problems with Product
- Produce wireframes, prototypes, and UI specs
- Define interaction and accessibility standards
- Validate usability before and after release
- Maintain design consistency

### Goals
- Usable, accessible, and consistent product experiences
- Reduce rework through early validation
- Improve customer satisfaction

### Typical Communication
- Design reviews and prototypes
- Specs and handoffs to Developers
- Usability findings shared with Product and QA

### How this role interacts with existing roles
- **Product Managers:** collaborates on problem framing and success metrics
- **Developers:** hands off specs and clarifies interaction details
- **QA / Test Engineers:** partners on usability acceptance

---

## DevOps / SRE

### Role Summary
DevOps/SRE engineers own CI/CD pipelines, deployment automation, observability, and incident-response readiness.

### Responsibilities
- Build and maintain CI/CD pipelines
- Automate deployments and rollbacks
- Instrument observability (errors, latency, usage)
- Prepare and run smoke tests and post-deploy verifications
- Lead incident response and on-call readiness
- Partner on security scanning in CI

### Goals
- Reliable, repeatable, low-risk releases
- Fast detection and recovery from incidents
- Strong observability and operational excellence

### Typical Communication
- Deployment and incident updates
- Runbooks and post-incident retrospectives
- Reliability and latency signals shared with the team

### How this role interacts with existing roles
- **Developers and Engineering Lead:** supports release and rollback per the [Release & Deployment guide](octoacme-release-and-deployment.md)
- **Project Managers:** provides reliability and latency signals and release status
- **Sponsors / Executive Stakeholders:** participates in incident communication when business impact is high

---

## Sponsors / Executive Stakeholders

### Role Summary
Sponsors provide funding, business alignment, and final go/no-go authority at decision gates.

### Responsibilities
- Approve scope, budget, and priorities
- Align project outcomes to business strategy
- Remove organizational blockers
- Serve as the top of the escalation path for business-impacting issues
- Make go/no-go decisions at gates

### Goals
- Ensure business value and ROI
- Maintain strategic alignment
- Enable timely decisions

### Typical Communication
- Milestone and decision-gate reviews
- Executive summaries and stakeholder briefings
- Escalation discussions

### How this role interacts with existing roles
- **Product Managers:** aligns on outcomes and priorities
- **Project Managers:** receives milestone updates and serves as the final escalation point per the escalation path Team-level → PM → Product Lead → Sponsor (see [Risks & Communication](octoacme-risks-and-communication.md) and [Execution & Tracking](octoacme-execution-and-tracking.md))

---

## Support / Customer Success

### Role Summary
Support and Customer Success teams represent the voice of the customer post-release and channel production feedback back into the backlog.

### Responsibilities
- Triage and route customer-reported issues
- Capture themes and feature requests
- Communicate known issues and workarounds
- Coordinate with DevOps/SRE during incidents
- Consume and relay release notes to customers

### Goals
- Fast resolution of customer issues
- Close the feedback loop into the backlog
- High customer satisfaction and retention

### Typical Communication
- Customer issue reports and summaries
- Incident status updates to customers
- Feedback themes shared with Product

### How this role interacts with existing roles
- **Product Managers:** feeds customer issues and themes into the backlog
- **DevOps / SRE:** coordinates during incidents (see [Release & Deployment guide](octoacme-release-and-deployment.md))
- **Project Managers:** consumes release notes from the release process

---

## Roles at a Glance

The table below maps each role to the primary lifecycle phases where it is most active. This is a lightweight reference; full responsibilities are defined in each persona section above and cross-referenced in related process docs.

| Role | Initiation | Planning | Execution | Release | Retrospective |
|---|---|---|---|---|---|
| Developers | | ✓ | ✓ | ✓ | ✓ |
| Product Managers | ✓ | ✓ | ✓ | ✓ | ✓ |
| Project Managers | ✓ | ✓ | ✓ | ✓ | ✓ |
| QA / Test Engineers | | ✓ | ✓ | ✓ | ✓ |
| Engineering Lead / Tech Lead | ✓ | ✓ | ✓ | ✓ | ✓ |
| Designers (UX/UI) | ✓ | ✓ | ✓ | | ✓ |
| DevOps / SRE | | ✓ | ✓ | ✓ | ✓ |
| Sponsors / Executive Stakeholders | ✓ | ✓ | | ✓ | |
| Support / Customer Success | | | | ✓ | ✓ |

See also: [Project Management Overview](octoacme-project-management-overview.md) · [Execution & Tracking](octoacme-execution-and-tracking.md) · [Risks & Communication](octoacme-risks-and-communication.md) · [Release & Deployment](octoacme-release-and-deployment.md)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

