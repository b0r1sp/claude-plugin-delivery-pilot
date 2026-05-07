---
name: status
description: Create or update a structured project status report. Use when asked for a project status, health check, RAG status, weekly status, or "how is the project going". Also triggers on "give me a status update" or "what's the current state".
argument-hint: "[project name or context]"
---

# /delivery-pilot:status

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Generate a structured project status report for stakeholders or leadership. See the **risks** skill for risk matrix frameworks and **timeline** for milestone details.

## Usage

```
/delivery-pilot:status $ARGUMENTS
```

## Output

```markdown
**Project:** [Name]
**Date:** [today]

| Area     | Status   | Comment |
|----------|----------|---------|
| Scope    | 🟢/🟡/🔴 |         |
| Timeline | 🟢/🟡/🔴 |         |
| Budget   | 🟢/🟡/🔴 |         |
| Risks    | 🟢/🟡/🔴 |         |
| Team     | 🟢/🟡/🔴 |         |

**Next Steps:**
1.
2.
3.
```

## If Connectors Available

If **~~project tracker** is connected:
- Pull current task status, completed items, and overdue work automatically
- Identify at-risk milestones and blockers

If **~~chat** is connected:
- Scan recent discussions for decisions and blockers to include
- Offer to post the finished status to a channel

## Tips

1. **Be honest about risks** — Surfacing issues early builds trust. Surprises erode it.
2. **Lead with the headline** — Busy stakeholders read the first few lines. Make them count.
3. **Pair with /delivery-pilot:risks** for a full picture of threats and mitigations.
