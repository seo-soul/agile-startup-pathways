# Glossary

Key terms you'll encounter in daily work, standups, and planning sessions. When in doubt, ask — but this reference should cover most of what you'll hear in your first few weeks.

---

## Agile

**Agile**
An umbrella term for iterative, team-centric approaches to software development. Not a specific framework — a set of values and principles articulated in the Agile Manifesto (2001).

**Backlog**
An ordered list of work items (stories, bugs, tasks) for a product or team. The Product Backlog is the full list; the Sprint Backlog is the subset planned for a given sprint.

**Backlog Refinement (Grooming)**
A recurring meeting where the team reviews, clarifies, and estimates upcoming backlog items. Keeps the backlog ready for the next sprint planning session.

**Definition of Done (DoD)**
A shared, explicit checklist of criteria that must be met before a work item can be considered complete. Prevents different interpretations of "done."

**Definition of Ready (DoR)**
Criteria that a backlog item must meet before it can be brought into a sprint. Typically includes: clearly described, estimated, and testable.

**Epic**
A large body of work that can be broken down into smaller stories. Epics may span multiple sprints.

**Increment**
The sum of all completed product backlog items at the end of a sprint. Should always be in a releasable state.

**Retrospective (Retro)**
A ceremony held at the end of each sprint where the team reflects on their process and identifies improvements.

**Sprint**
A fixed-length iteration (typically 1–4 weeks) during which a team completes a set of planned work items.

**Sprint Goal**
A single, concise statement of what the team intends to achieve during a sprint. Gives the sprint coherence and focus.

**Story Points**
A relative unit of effort estimation. Not hours — they capture complexity, uncertainty, and effort together. Teams calibrate their own scale.

**User Story**
A short description of a feature from the perspective of an end user. Format: *"As a [user], I want [feature], so that [benefit]."*

**Velocity**
The average number of story points a team completes per sprint. Used for capacity planning, not comparison between teams.

---

## Scrum Roles

**Product Owner (PO)**
Responsible for the product backlog and for maximizing the value delivered by the team. Defines what gets built and in what order.

**Scrum Master (SM)**
Facilitates the Scrum process, removes impediments, and helps the team continuously improve. Not a project manager.

**Development Team**
The cross-functional group of individuals who deliver the product increment each sprint. Self-organizing and collectively responsible.

---

## Kanban

**Kanban Board**
A visual board with columns representing workflow stages (e.g., To Do → In Progress → Review → Done). Work items move left to right.

**WIP Limit (Work In Progress Limit)**
A cap on the number of items allowed in a given workflow stage at once. Prevents overloading and exposes bottlenecks.

**Lead Time**
Total time from when a work item is requested to when it is delivered.

**Cycle Time**
Time from when work actually begins on an item to when it is completed. A subset of lead time.

**Throughput**
The number of items completed per unit of time. A key flow metric.

---

## Engineering

**CI/CD**
Continuous Integration / Continuous Delivery (or Deployment). The practice of automatically building, testing, and deploying code changes.

**Code Review (PR Review)**
The process of having peers examine proposed code changes before they are merged. Catches bugs, spreads knowledge, and improves quality.

**Pair Programming**
Two developers working together at one machine — one "drives" (writes code), one "navigates" (reviews and thinks ahead).

**Refactoring**
Changing the internal structure of code without changing its external behavior. Improves readability and maintainability.

**Technical Debt**
The implied cost of shortcuts or suboptimal decisions made to ship faster. Not inherently bad — but it compounds if left unmanaged.

**TDD (Test-Driven Development)**
Writing tests before writing the production code that makes them pass. Red → Green → Refactor cycle.

---

## Delivery & Metrics

**DORA Metrics**
Four key metrics that predict software delivery performance:
1. Deployment Frequency
2. Lead Time for Changes
3. Mean Time to Recovery (MTTR)
4. Change Failure Rate

**Feature Flag**
A configuration mechanism that enables or disables a feature at runtime without deploying new code.

**MVP (Minimum Viable Product)**
The smallest version of a product that delivers enough value to validate a hypothesis or learn from real users.

**SLA / SLO / SLI**
- **SLI** (Service Level Indicator): A metric measuring service behavior (e.g., latency, error rate)
- **SLO** (Service Level Objective): A target value for an SLI
- **SLA** (Service Level Agreement): A contract specifying consequences if SLOs are not met

---

## Communication

**ADR (Architecture Decision Record)**
A short document capturing an architectural decision, its context, and its rationale. Helps future team members understand why things were built the way they were.

**Blocker**
Anything preventing a team member from progressing on their work. Raised in standup; the Scrum Master helps resolve it.

**Impediment**
Similar to a blocker, but sometimes used more broadly to include inefficiencies or friction that slow the team down without fully stopping them.

**Standup / Daily Scrum**
A brief (15-minute max) daily check-in. Classic format: What did I do yesterday? What will I do today? Any blockers?
