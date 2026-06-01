# Task Deletion

## Feature Added

The Task Deletion feature allows users to remove tasks that are no longer needed.

This helps keep the dashboard organized and ensures that outdated or unnecessary work items do not clutter the project workflow.

---

## Code Used

```javascript
const deleteTask = (id) => {
  setTasks(
    tasks.filter(task => task.id !== id)
  )
}
```

---

## What The Code Does

This function removes a task from the task list by filtering out the selected task ID.

After the task is removed, React automatically updates the dashboard and task counts.

---

## Why I Implemented It

Project management tools need a way to remove completed, cancelled, or incorrect tasks.

Without task deletion, the dashboard would eventually become cluttered and difficult to manage.

---

## Impact On The Application

This feature allows users to:

- Remove unnecessary tasks
- Keep project boards organized
- Maintain accurate task counts
- Improve workflow management

---

## Business Value

Task deletion improves data accuracy and dashboard organization.

By allowing users to remove outdated work items, the application remains focused on active and relevant project tasks.
