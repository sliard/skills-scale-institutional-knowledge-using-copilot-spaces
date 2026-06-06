# OctoAcme — Cross-Role Responsibility Matrix & Handoff Guide

## Purpose
Provide a concise reference showing who owns, contributes to, and must be consulted or informed at each phase of the OctoAcme project lifecycle. Use this alongside the individual role definitions in `octoacme-roles-and-personas.md`.

## RACI Key
| Symbol | Meaning |
|---|---|
| **R** | Responsible — does the work |
| **A** | Accountable — final decision / sign-off |
| **C** | Consulted — input required before action |
| **I** | Informed — kept up-to-date on progress or outcomes |

---

## Lifecycle Phase Responsibility Matrix

| Activity | PM | PdM | Dev | UX | DevOps | BA | Support Lead | QA |
|---|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | | |
| Draft project one-pager | A | R | I | C | I | C | I | I |
| Stakeholder alignment | A | R | I | I | I | C | C | I |
| Approve go/no-go | A | A | I | I | I | I | I | I |
| **Planning** | | | | | | | | |
| Requirements elicitation | C | A | C | C | I | R | C | C |
| Backlog creation & prioritization | C | A | C | C | I | R | C | I |
| UX design & prototyping | I | A | C | R | I | C | I | I |
| Acceptance criteria authoring | I | A | C | C | I | R | C | C |
| Effort estimation | R | C | R | R | C | C | I | C |
| Release plan & milestones | A | C | C | I | C | I | I | I |
| Definition of Done | R | A | C | C | C | C | I | R |
| **Execution** | | | | | | | | |
| Feature development | I | A | R | C | C | I | I | I |
| Design review / implementation sign-off | I | C | R | A | I | I | I | I |
| CI/CD pipeline & environment support | A | I | C | I | R | I | I | C |
| PR review & merge | I | I | A | I | C | I | I | C |
| Daily standup facilitation | R | I | R | R | I | I | I | I |
| Risk register updates | R | C | C | I | C | C | I | I |
| **Quality & Testing** | | | | | | | | |
| Test plan authoring | C | I | C | C | I | C | I | A |
| Feature acceptance testing | I | A | C | C | I | C | I | R |
| Accessibility / UX validation | I | C | C | A | I | I | I | R |
| Security / compliance scans | A | I | C | I | R | I | I | C |
| **Release** | | | | | | | | |
| Release readiness sign-off | A | C | C | C | R | I | C | R |
| Deployment execution | A | I | C | I | R | I | I | C |
| Release notes authoring | R | C | C | I | C | C | R | I |
| Support team briefing | A | I | I | I | C | I | R | I |
| Post-deploy verification | C | I | C | I | R | I | C | R |
| **Retrospective** | | | | | | | | |
| Retrospective facilitation | A | C | R | R | R | R | R | R |
| Action items: capture & assign | A | C | C | C | C | C | C | C |
| Action items: follow-up | R | C | C | C | C | C | C | C |
| Feedback digest to team | I | A | I | I | I | I | R | I |

---

## Key Handoff Points

### 1. Initiation → Planning
**Handoff from:** Product Manager + Project Manager  
**Handoff to:** Business Analyst, UX Designer  
**Deliverables passed on:**
- Approved project one-pager
- Stakeholder list and communication plan
- Initial risk list

**Checklist:**
- [ ] One-pager signed off by Product Manager and sponsor
- [ ] BA briefed on business context and constraints
- [ ] UX Designer briefed on user research needs
- [ ] Project board / repo skeleton created

---

### 2. Planning → Execution
**Handoff from:** Business Analyst, UX Designer, Product Manager  
**Handoff to:** Developers, QA  
**Deliverables passed on:**
- Prioritized backlog with acceptance criteria
- Finalized design specs and prototypes
- Definition of Done
- Initial risk register

**Checklist:**
- [ ] All sprint-1 backlog items have written acceptance criteria (BA sign-off)
- [ ] Design specs linked to backlog items (UX sign-off)
- [ ] QA has reviewed acceptance criteria and started test plan
- [ ] DevOps has confirmed environment readiness
- [ ] PM has confirmed team capacity and sprint goal

---

### 3. Execution → Release
**Handoff from:** Developers, QA  
**Handoff to:** DevOps Engineer, Customer Support Lead, Project Manager  
**Deliverables passed on:**
- Merged and tested code
- Passing CI and security scans
- Draft release notes
- Rollback plan

**Checklist:**
- [ ] All acceptance criteria verified by QA
- [ ] Release notes drafted and reviewed by PM + Support Lead
- [ ] DevOps confirms deployment window and rollback plan
- [ ] Support Lead confirms support team is briefed
- [ ] Smoke-test script prepared

---

### 4. Release → Retrospective
**Handoff from:** Project Manager, DevOps Engineer  
**Handoff to:** Full team  
**Deliverables passed on:**
- Post-deploy verification results
- Incident or anomaly log (if any)
- Support ticket trend data (from Support Lead)

**Checklist:**
- [ ] Post-deploy metrics reviewed
- [ ] Any incidents logged with action items
- [ ] Retrospective scheduled and facilitated by PM
- [ ] Customer Support Lead shares feedback digest
- [ ] Action items captured, owned, and added to backlog

---

## Communication Touchpoints by Role

| Role | Key recurring touchpoints |
|---|---|
| Project Manager | Weekly status report; risk register review; sprint planning & retro facilitation |
| Product Manager | Roadmap review (monthly); backlog refinement (weekly); stakeholder briefing (milestone) |
| UX Designer | Design critique (per sprint); handoff review with Developers (per feature) |
| DevOps Engineer | Release readiness review (per release); incident retrospective (as needed) |
| Business Analyst | Requirements review before sprint commitment; stakeholder sign-off (per feature) |
| Customer Support Lead | Monthly feedback digest; release briefing (per release); retro participation |
| QA / Testing | Test plan review (per sprint); acceptance sign-off (per feature) |
| Developers | Daily standup; PR review; technical design doc (as needed) |

---

## Related Documents
- [OctoAcme Personas](./octoacme-roles-and-personas.md)
- [OctoAcme Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
