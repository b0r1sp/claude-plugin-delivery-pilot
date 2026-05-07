---
name: timeline
description: Create or update a milestone timeline. Use when planning milestones, checking delivery dates, asking "are we on track", or when someone needs a project timeline, roadmap overview, or wants to see upcoming dates.
argument-hint: "[project name, time range, or milestone]"
---

# /delivery-pilot:timeline

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Create or update a milestone timeline with critical path and delivery forecast. See **status** for overall project health and **estimate** for effort-based scheduling.

## Usage

```
/delivery-pilot:timeline $ARGUMENTS
```

## Output

```markdown
**Project:** [Name]

| Milestone | Planned | Forecast | Status   | Owner | Dependency |
|-----------|---------|----------|----------|-------|------------|
|           |         |          | 🟢/🟡/🔴 |       |            |

**Status:** 🟢 On Track · 🟡 At Risk · 🔴 Delayed · ✅ Done

**Critical Path:**
→ [Milestone 1] → [Milestone 2] → ...
```

## If Connectors Available

If **~~project tracker** is connected:
- Pull milestones, sprints, and due dates automatically
- Highlight overdue items and forecast slippage

If **~~calendar** is connected:
- Cross-reference key meetings, reviews, and deadlines
- Flag calendar conflicts with milestone dates

## Tips

1. **Mark the critical path explicitly** — Not all delays are equal. Only critical path delays affect the end date.
2. **Forecast ≠ Plan** — Always show both planned and forecast dates once slippage occurs.
3. **Pair with /delivery-pilot:risks** to connect timeline risks to the risk register.
