---
name: context-update
description: Update a team member's personal context entry with current focus, actions, and blockers. Use when someone wants to update their status, says "update my context", "I'm now working on", or at the start of a new week.
argument-hint: "[team member name]"
---

# /delivery-pilot:context-update

Keep the team context current. Profile fields (MBTI, CliftonStrengths, Skills) only change on explicit request — only the **Current** section is updated in a regular update.

## Usage

```
/delivery-pilot:context-update $ARGUMENTS
```

## Steps

1. Read `context/members/_template.md` as schema
2. Read existing `context/members/[name].md` if present
3. Ask for changes in the **Current** section (Focus, Actions, Blockers)
4. Write updated file to `context/members/[name].md`
5. Update the corresponding row in `context/members/team.md`

## If Connectors Available

If **~~chat** is connected:
- Pull recent messages from the team member to pre-fill focus and blockers
- Suggest updates based on what they've been discussing

If **~~project tracker** is connected:
- Pull assigned tasks and in-progress items to populate open actions

## Tips

1. **Update weekly** — Stale context leads to wrong assumptions in standup, handover, and escalation.
2. **Blockers are the most valuable field** — Make sure they're specific and actionable, not vague.
3. **Pair with /delivery-pilot:agile-standup** — standup reads from member context automatically.
