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

## UX Designer

### Role Summary
UX Designers research user needs, define interaction patterns, and produce design artefacts that guide development. They advocate for usability and accessibility throughout the product lifecycle.

### Responsibilities
- Conduct user research, usability tests, and heuristic reviews
- Produce wireframes, prototypes, and interaction specifications
- Maintain and evolve the design system and component library
- Review implemented features against design intent
- Champion accessibility (WCAG) and inclusive design

### Goals
- Ensure every shipped feature solves a real user problem
- Reduce rework caused by usability issues discovered late
- Provide clear, implementation-ready design artefacts

### Typical Communication
- Design reviews and critique sessions with Product Managers and Developers
- Handoff notes and annotated specs in the design tool (e.g., Figma)
- User research readouts shared with the broader team

### Role Interactions
| Role | Interaction |
|---|---|
| Product Manager | Aligns research findings with roadmap priorities; co-defines acceptance criteria for UX outcomes |
| Project Manager | Flags design-scope changes that affect timelines; participates in planning to size design tasks |
| Developers | Reviews implementations against specs; resolves design ambiguities during development |
| QA / Testing | Provides acceptance criteria for visual and interaction quality; validates accessibility |
| Stakeholders | Presents research findings and design rationale to gain alignment before build begins |

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the pipelines, infrastructure, and tooling that enable reliable, fast delivery. They bridge development and operations to maximize deployment confidence and system reliability.

### Responsibilities
- Design and maintain CI/CD pipelines and deployment automation
- Manage infrastructure-as-code (IaC) and cloud environments
- Monitor system health, set up alerting, and respond to incidents
- Enforce security scanning, secrets management, and compliance controls in pipelines
- Advise on release readiness and operational risk

### Goals
- Achieve fast, repeatable, and low-risk deployments
- Minimize mean time to recovery (MTTR) for production incidents
- Provide developers with self-service tooling for builds and deployments

### Typical Communication
- Release readiness sign-off with Project Manager before each deployment
- Incident updates and post-mortems shared with the full team
- Infrastructure change proposals reviewed asynchronously via PRs

### Role Interactions
| Role | Interaction |
|---|---|
| Product Manager | Communicates operational constraints and platform capacity that may affect roadmap timing |
| Project Manager | Provides deployment-window estimates and flags infrastructure risks for the risk register |
| Developers | Reviews application code for deploy-time concerns (env config, migrations, feature flags); supports local dev tooling |
| QA / Testing | Provisions staging environments; supports test-data seeding and smoke-test automation |
| Stakeholders | Presents reliability metrics and incident summaries at major milestones |

---

## Business Analyst

### Role Summary
Business Analysts gather, structure, and clarify requirements, acting as the bridge between stakeholders and the delivery team. They ensure that acceptance criteria are complete and unambiguous before development begins.

### Responsibilities
- Facilitate requirements workshops and elicitation sessions with stakeholders
- Author detailed user stories, use cases, and acceptance criteria
- Maintain a requirements traceability matrix linking business needs to backlog items
- Validate delivered features against business requirements
- Document process flows and data mappings for complex features

### Goals
- Eliminate requirements ambiguity that causes rework during development
- Ensure all in-scope business needs are traceable to backlog items
- Support a shared understanding of "done" across the team

### Typical Communication
- Requirements review sessions with Product Manager and Developers before sprint commitment
- Written acceptance criteria and process-flow diagrams attached to backlog items
- Stakeholder sign-off confirmations captured in writing

### Role Interactions
| Role | Interaction |
|---|---|
| Product Manager | Translates product vision and user research into structured requirements; aligns on backlog priority |
| Project Manager | Flags scope creep early; provides effort-impact analysis to support scheduling decisions |
| Developers | Clarifies acceptance criteria and edge cases during sprint; reviews implementation for requirements completeness |
| QA / Testing | Co-creates test scenarios from acceptance criteria; validates that test coverage matches business requirements |
| Stakeholders | Facilitates workshops to capture needs; seeks formal sign-off on documented requirements |

---

## Customer Support Lead

### Role Summary
Customer Support Leads represent the voice of the customer within the product team. They surface customer-reported pain points, track bug trends, and ensure support readiness for each release.

### Responsibilities
- Aggregate and prioritize customer feedback and bug reports for product review
- Communicate known issues, workarounds, and release impacts to the support team
- Participate in sprint demos and retrospectives to provide customer-facing perspective
- Maintain and update user-facing release notes and support articles
- Track customer satisfaction metrics and escalate critical issues to Product Managers

### Goals
- Reduce support ticket volume by influencing fixes for top reported issues
- Ensure the support team is prepared for every release
- Close the feedback loop between customers and the delivery team

### Typical Communication
- Monthly feedback digest shared with Product Manager and Project Manager
- Release readiness briefing to the support team before each deployment
- Escalation tickets raised directly with the Product Manager for critical customer-impacting issues

### Role Interactions
| Role | Interaction |
|---|---|
| Product Manager | Provides quantified customer feedback to inform backlog prioritization; escalates critical defects |
| Project Manager | Raises support-readiness risk ahead of releases; confirms that user-facing documentation is complete |
| Developers | Reports reproducible bugs with supporting data; validates bug fixes from a customer-use-case perspective |
| QA / Testing | Contributes real-world user scenarios and edge cases to the test plan |
| Stakeholders | Shares customer satisfaction data and support trends at milestone reviews |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See `octoacme-raci-and-handoffs.md` for a cross-role responsibility matrix across project lifecycle phases.

