# Local Storage

## Feature Added

The Local Storage feature allows TaskFlow to save task data directly in the user's browser.

This ensures that tasks remain available even after the page is refreshed or the browser is closed and reopened.

---

## Code Used

```javascript
useEffect(() => {
  localStorage.setItem(
    'taskflowTasks',
    JSON.stringify(tasks)
  )
}, [tasks])
```

---

## What The Code Does

This code monitors the task list for changes.

Whenever a task is created, updated, moved, or deleted, the current task data is converted into a JSON string and stored in the browser's local storage.

The saved data can then be retrieved when the application loads.

---

## Why I Implemented It

Without local storage, all task data would be lost whenever the page was refreshed.

I wanted users to have a persistent experience without requiring a backend database.

---

## Impact On The Application

This feature allows users to:

- Save tasks between sessions
- Refresh the page without losing data
- Continue working where they left off
- Improve overall user experience

---

## Business Value

Data persistence is an important feature in project management software.

By storing task information locally, users can reliably manage projects without worrying about losing their work.
