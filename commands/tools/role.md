# /role — Activate Role

Slip into a professional role to frame all subsequent commands from that role's perspective.

## Usage
- `/role [name]` — activate a role (e.g. `/role it-consultant`)
- `/role` — show the currently active role
- `/role off` — deactivate the current role

## Available Roles
Located in `context/roles/`. Current roles:
- `test-lead`
- `it-consultant`
- `infrastructure-specialist`

## Behavior

### Activating a role
1. Read the matching file from `context/roles/[name].md`
2. Write `context/roles/active-role.md` with role name, activation date, and profile path
3. Briefly introduce the role: name, perspective, and top 3 priorities
4. Confirm the role is active

### Showing active role
1. Read `context/roles/active-role.md`
2. Display role name, activation date, and key characteristics
3. If no role is active, say so and list available roles

### Deactivating
1. Delete or clear `context/roles/active-role.md`
2. Confirm role has been deactivated

## Effect on other commands
When a role is active, commands like `/research`, `/update`, and `/reporting`
read `context/active-role.md` and adapt their perspective, priorities, and
output style accordingly.
