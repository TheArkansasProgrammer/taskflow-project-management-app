# Task Creation

## Feature Added

The Task Creation feature allows users to add new tasks directly from the dashboard.

This transformed TaskFlow from a static dashboard into an interactive project management application.

---

## Code Used

```javascript
const addTask = () => {
  if (!newTask.trim()) return

  setTasks([
    ...tasks,
    {
      id: Date.now(),
      title: newTask,
      status: 'todo',
      priority,
      dueDate,
    },
  ])

  setNewTask('')
  setPriority('Medium')
  setDueDate('')
}
```

---

## What The Code Does

This function creates a new task object using information entered by the user.

The task is assigned:

- A unique ID
- A title
- A status
- A priority level
- A due date

The task is then added to the existing task list and immediately displayed on the dashboard.

---

## Why I Implemented It

A project management tool must allow users to create and organize work items.

Without task creation, users would only be able to view pre-existing tasks and could not actively manage projects.

---

## Impact On The Application

This feature allows users to:

- Create new tasks
- Organize project work
- Build project workflows
- Track progress from start to completion

---

## Business Value

Task creation is one of the most important features in any project management system.

It enables teams to capture work, organize responsibilities, and track progress throughout the project lifecycle.
