# Task Status Updates

## Feature Added

The Task Status Updates feature allows users to move tasks between workflow stages as work progresses.

Tasks can move between:

- To Do
- In Progress
- Done

This allows the dashboard to accurately reflect project progress.

---

## Code Used

```javascript
const updateStatus = (id, newStatus) => {
  setTasks(
    tasks.map(task =>
      task.id === id
        ? { ...task, status: newStatus }
        : task
    )
  )
}
```

---

## What The Code Does

This function searches for the selected task and updates its status.

When a user changes the task status, the task is automatically moved to the appropriate Kanban board column.

The dashboard metrics are also updated automatically.

---

## Why I Implemented It

A project management application should allow work to move through different stages.

Without status updates, tasks would remain permanently stuck in their original workflow column.

---

## Impact On The Application

This feature allows users to:

- Track project progress
- Move work between stages
- Update project status
- Manage workflows more effectively

---

## Business Value

Status tracking is a core component of project management.

It allows teams to understand what work has started, what work is currently being completed, and what work has been finished.
