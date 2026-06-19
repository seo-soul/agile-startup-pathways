# Kanban

Kanban is a flow-based approach to managing and improving work. Unlike Scrum, it has no prescribed roles, fixed-length iterations, or mandatory ceremonies. It works by making work visible, limiting work in progress, and continuously improving flow.

> "Stop starting, start finishing."
> — Kanban mantra

---

## Origins

Kanban was developed by Taiichi Ohno at Toyota in the 1950s as part of the Toyota Production System. David Anderson adapted it for software development in the 2000s, codifying what is now known as the Kanban Method.

---

## Core Practices

### 1. Visualize the Workflow

Create a board with columns representing each state in your process:

```
Backlog → Ready → In Progress → Review → Done
```

Each work item is a card that moves left to right. Visualization makes invisible work visible and exposes bottlenecks.

### 2. Limit Work in Progress (WIP)

Assign a maximum number of items allowed in each column. When a column is full, team members pull from an earlier stage or help unblock existing work rather than starting something new.

**Why it works:** WIP limits prevent multitasking, reduce context switching, and force conversations about priorities. They surface bottlenecks that would otherwise stay hidden.

### 3. Manage Flow

Monitor how work moves through the system. Look for:
- Items stuck in a column for too long
- Columns consistently hitting their WIP limits
- Patterns in what type of work causes delays

### 4. Make Policies Explicit

Document and post your workflow rules: What does "Ready" mean? When does something move to Review? Who can pull what? Explicit policies reduce friction and enable self-management.

### 5. Implement Feedback Loops

Regular reviews of flow metrics and team process — even without fixed sprint timelines. Common cadences include weekly flow reviews and monthly retrospectives.

### 6. Improve Collaboratively, Evolve Experimentally

Use data and shared understanding to drive incremental improvement. Small, reversible experiments. Measure the impact. Adjust.

---

## Key Metrics

**Lead Time** — Total elapsed time from when a request is made to when it is delivered. Includes wait time.

**Cycle Time** — Time from when work actually starts to when it is finished. The part the team controls.

**Throughput** — Number of items completed per unit of time (e.g., 12 stories per week). A key capacity metric.

**WIP** — Current count of items in progress. High WIP = high context switching = slower cycle times.

**Cumulative Flow Diagram (CFD)** — A stacked area chart showing the count of items in each workflow state over time. Healthy CFDs show smooth, parallel bands. Widening bands indicate growing queues.

---

## Kanban vs. Scrum

| | Scrum | Kanban |
|-|-------|--------|
| **Cadence** | Fixed sprints | Continuous flow |
| **Roles** | PO, SM, Developers | No prescribed roles |
| **Change** | No changes mid-sprint | Can be added anytime |
| **Estimation** | Story points (typical) | Optional |
| **Primary metric** | Velocity | Cycle time / throughput |
| **Best for** | Feature development | Support, ops, maintenance |

These are not mutually exclusive. **Scrumban** combines sprint structure with WIP limits and flow metrics.

---

## When Kanban Makes Sense

Kanban tends to work well when:
- Work arrives unpredictably (support, bug fixes, ops tasks)
- Items vary widely in size and urgency
- The team wants to start with minimal process change
- You need to visualize and improve an existing workflow without restructuring the team

---

## Further Reading

- *Kanban: Successful Evolutionary Change for Your Technology Business* — David J. Anderson
- *Kanban from the Inside* — Mike Burrows
- [kanban.university](https://kanban.university) — Official Kanban Method resources
