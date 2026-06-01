# Due Date Tracking

## Feature Added

The Due Date Tracking feature allows users to assign deadlines to tasks.

This helps users plan work, manage schedules, and track upcoming project milestones.

---

## Code Used

```javascript
const [dueDate, setDueDate] = useState('')

<input
  type="date"
  value={dueDate}
  onChange={(e) => setDueDate(e.target.value)}
/>
```

---

## What The Code Does

This code allows users to select a date when creating a task.

The selected date is stored with the task information and displayed on the dashboard.

---

## Why I Implemented It

Project tasks often have deadlines and target completion dates.

Adding due dates makes it easier to organize work and plan project timelines.

---

## Impact On The Application

This feature allows users to:

- Assign deadlines to tasks
- Track project milestones
- Improve project planning
- Monitor upcoming work

---

## Business Value

Due date tracking improves scheduling and accountability.

By providing visibility into deadlines, users can better manage workloads and reduce the risk of missed project milestones.
