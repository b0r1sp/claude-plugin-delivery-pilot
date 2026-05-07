---
name: agile-retrospective
description: Facilitate or prepare a sprint retrospective. Use when a sprint or iteration ends and the team wants to reflect, or when asked for a retro, retrospective, "what went well", "what should we improve", or "lessons learned".
argument-hint: "[sprint number or team name]"
---

# /delivery-pilot:agile-retrospective

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Facilitate a retrospective using the Start / Stop / Continue format. Closes with concrete action items. See **/delivery-pilot:agile-standup** for sprint-level context.

## Usage

```
/delivery-pilot:agile-retrospective $ARGUMENTS
```

## Output

```markdown
**Retrospective – [Sprint/Team]**

### 🟢 Continue — What worked well?
-

### 🔴 Stop — What should we stop doing?
-

### 🟡 Start — What should we try?
-

---

## Action Items

| Action | Owner | Due | Status |
|--------|-------|-----|--------|
|        |       |     | Open   |

**Team mood:** 😞 😐 🙂 😄 (Average: )
```

## If Connectors Available

If **~~project tracker** is connected:
- Pull sprint metrics (velocity, completed vs. planned, carry-overs) as input
- Create action item tickets directly from the retro

If **~~chat** is connected:
- Post the retro summary to the team channel

## Tips

1. **End with actions, not feelings** — A retro without action items is just venting.
2. **Limit actions** — 1–3 concrete actions per retro. More than that and nothing gets done.
3. **Review previous retro actions first** — Did last sprint's actions actually happen?
