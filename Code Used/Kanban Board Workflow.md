# Kanban Board Workflow

## Feature Added

The Kanban Board Workflow organizes tasks into three project stages:

- To Do
- In Progress
- Done

This provides users with a visual representation of project progress and task status.

---

## Code Used

```javascript
const renderTasks = (status) =>
  tasks
    .filter(task => task.status === status)
    .map(task => (
      <div className="task" key={task.id}>
        {task.title}
      </div>
    ))
```

---

## What The Code Does

This code filters tasks based on their current status and displays them in the appropriate workflow column.

Tasks marked as:

- todo appear in the To Do column
- progress appear in the In Progress column
- done appear in the Done column

The board updates automatically whenever task statuses change.

---

## Why I Implemented It

I wanted users to visually track work as it moves through the project lifecycle.

A Kanban board provides a simple and effective way to organize tasks and monitor progress.

---

## Impact On The Application

This feature allows users to:

- Visualize project progress
- Organize work stages
- Identify tasks currently being worked on
- Track completed work

---

## Business Value

Kanban workflows are widely used in project management because they improve visibility and team organization.

This feature helps users understand project status at a glance and supports better workload management.
