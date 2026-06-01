# Dashboard Metrics

## Feature Added

The Dashboard Metrics feature provides users with a real-time overview of project progress by displaying task statistics directly on the dashboard.

The metrics update automatically whenever tasks are created, completed, or deleted.

---

## Code Used

```javascript
const totalTasks = tasks.length

const completedTasks =
  tasks.filter(task => task.status === 'done').length

const pendingTasks =
  totalTasks - completedTasks
```

---

## What The Code Does

This code calculates three key project statistics:

- Total Tasks
- Completed Tasks
- Pending Tasks

The values are generated dynamically using the current task data stored within the application.

Whenever the task list changes, the dashboard metrics update automatically.

---

## Why I Implemented It

Project managers and team members need quick visibility into project progress.

Instead of manually counting tasks, the dashboard automatically summarizes project status.

---

## Impact On The Application

This feature allows users to:

- Monitor overall project progress
- Track completed work
- Identify remaining workload
- Quickly assess project status

---

## Business Value

Dashboard metrics improve visibility and decision-making.

By providing instant access to project statistics, users can better understand progress, identify bottlenecks, and make informed project management decisions.
