# Schema Draft

## Roadmap
- **title**: string, required
- **description**: text
- **outcomes**: text or structured list
- **timeline_start**: date/datetime
- **timeline_end**: date/datetime
- **owner_admin_id**: foreign key to user/admin
- **visibility**: enum (e.g., private, team, public)
- **slug**: string, unique

## Milestone
- **title**: string, required
- **description**: text
- **order**: integer
- **target_date**: date/datetime
- **completion_rules**: text or structured ruleset

## Task
- **title**: string, required
- **details**: text
- **checklist_state**: enum or JSON (e.g., items with done flags)
- **created_at**: datetime
- **updated_at**: datetime
- **completed_at**: datetime, nullable

## Progress
- **progress_percent**: computed dynamically from completed tasks/milestones (not stored).
