---
name: agile-standup
description: Prepare or facilitate a daily standup. Use when asked for a standup, daily sync, "what did we do yesterday", sprint check-in, or morning team update.
argument-hint: "[team name or sprint context]"
---

# /delivery-pilot:agile-standup

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Prepare or run the daily standup. Reads from `context/members/` for current focus and blockers. Use **/delivery-pilot:context-update** to keep member context fresh.

## Usage

```
/delivery-pilot:agile-standup $ARGUMENTS
```

## Structure (per team member)

1. **Yesterday:** What was completed?
2. **Today:** What is planned?
3. **Blockers:** Any impediments?

## Output

```markdown
**Standup – [Date] · [Team/Sprint]**

| Person | Yesterday | Today | Blockers |
|--------|-----------|-------|----------|

**Delivery Lead Note:**
- Blockers:
- Risks:
- Escalation needed:
```

## If Connectors Available

If **~~project tracker** is connected:
- Pull completed and in-progress tasks per person automatically
- Flag overdue items as blockers

If **~~chat** is connected:
- Post the standup summary to the team channel after completion

## Tips

1. **Timebox ruthlessly** — Standups are status, not problem-solving. Park deep discussions.
2. **Focus on blockers** — That's the one thing a Delivery Lead can act on immediately.
3. **Pair with /delivery-pilot:risks** — New blockers often become risks.
