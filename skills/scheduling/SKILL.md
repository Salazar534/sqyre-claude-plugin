---
name: scheduling
description: Use when the user asks what is on the Sqyre calendar, or wants a visit scheduled, moved, assigned, or completed.
---

# Sqyre schedule

Use Sqyre MCP tools only. Never invent visit ids or worker ids.

Read the board with `get_today_schedule`, `get_tomorrow_schedule`, `get_calendar`, `get_calendar_day`, `list_visits`, and `get_unassigned_visits`. Use `get_visit` before changing one visit.

Resolve the client and project before `schedule_visit`. Check `check_schedule_conflicts` and `get_available_workers` or `get_worker_schedule` before assigning someone.

`reschedule_visit`, `cancel_visit`, `assign_worker_to_visit`, `unassign_worker_from_visit`, `mark_visit_confirmed`, and `mark_visit_complete` each need the visit id from a read, not from memory. After a change, read the visit again and tell the user the date and worker Sqyre stored.
