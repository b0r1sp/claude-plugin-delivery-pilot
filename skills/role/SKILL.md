---
name: role
description: Activate a professional role to frame subsequent commands from that role's perspective. Use when asked to "act as", "think like a", "from the perspective of", or when switching roles like IT consultant, test lead, or infrastructure specialist.
argument-hint: "[role name | 'off']"
---

# /delivery-pilot:role

Slip into a professional role. All subsequent commands — especially **/delivery-pilot:research** — adapt their perspective, questions, frameworks, and output style to the active role.

## Usage

```
/delivery-pilot:role [name]     # activate a role
/delivery-pilot:role            # show active role
/delivery-pilot:role off        # deactivate
```

## Available Roles

Located in `context/roles/`:

| Role | Focus |
|------|-------|
| `test-lead` | Quality, coverage, risk-based testing |
| `it-consultant` | Technology strategy, architecture, trade-offs |
| `infrastructure-specialist` | Reliability, security, scalability |

## Behavior

**Activating:**
1. Read `context/roles/[name].md`
2. Write `context/roles/active-role.md` with role name, activation date, profile path
3. Briefly introduce the role: name, perspective, top 3 priorities

**Showing active role:**
1. Read `context/roles/active-role.md`
2. Display role name, activation date, key characteristics
3. If none active, list available roles

**Deactivating:**
1. Clear `context/roles/active-role.md`
2. Confirm deactivation

## Tips

1. **Activate before researching** — `/delivery-pilot:role it-consultant` then `/delivery-pilot:research` gives a fundamentally different analysis.
2. **New roles** — Copy `context/roles/_template.md`, fill in all sections including Behavioral Guidelines.
3. **One role at a time** — Roles are mutually exclusive. Activating a new one replaces the previous.
