# Priority Management

## Feature Added

The Priority Management feature allows users to assign importance levels to tasks.

Tasks can be categorized as:

- High Priority
- Medium Priority
- Low Priority

This helps users focus on the most important work first.

---

## Code Used

```javascript
const [priority, setPriority] = useState('Medium')

<select
  value={priority}
  onChange={(e) => setPriority(e.target.value)}
>
  <option>Low</option>
  <option>Medium</option>
  <option>High</option>
</select>
```

---

## What The Code Does

This code allows users to select a priority level when creating a task.

The selected priority is stored with the task data and displayed on the Kanban board.

---

## Why I Implemented It

Not every task has the same level of importance.

Users need a way to identify critical work and prioritize their workload accordingly.

---

## Impact On The Application

This feature allows users to:

- Prioritize important tasks
- Organize workloads more effectively
- Focus on high-impact work
- Improve project planning

---

## Business Value

Prioritization helps teams allocate time and resources efficiently.

By identifying important tasks, users can focus on the work that delivers the greatest value to the project.
