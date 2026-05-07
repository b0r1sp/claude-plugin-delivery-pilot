---
name: escalate
description: Formulate a clear, professional escalation message. Use when something is blocked, at risk, or needs urgent decision, or when asked to "escalate", "write an escalation", "flag this to management", or "this needs to go up".
argument-hint: "[topic or recipient]"
---

# /delivery-pilot:escalate

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Structure an escalation with facts, impact, and a clear ask. See **/delivery-pilot:risks** for the risk context and **/delivery-pilot:update** for less urgent communications.

## Principles

- Facts over emotions
- Clearly separate problem, impact, and required action
- Provide solution options — not just the escalation
- State urgency and decision deadline explicitly

## Usage

```
/delivery-pilot:escalate $ARGUMENTS
```

## Output

```markdown
**Escalation – [Date]**
**Topic:** [Topic]
**Urgency:** High / Medium

---

**Situation:**
[What happened? Facts, data, timeline]

**Impact:**
[What happens if no action is taken? Cost, risk, delay]

**Actions taken so far:**
-

**Decision / Support requested:**
- [ ] Option A:
- [ ] Option B:

**Decision deadline:**
```

## If Connectors Available

If **~~email** is connected:
- Draft the escalation as a ready-to-send email

If **~~calendar** is connected:
- Check the recipient's availability and suggest a meeting slot if needed

## Tips

1. **Lead with the ask** — Busy executives read the first paragraph. Put the decision needed there.
2. **Bring solutions, not just problems** — "Here are two options" is much stronger than "we have a problem".
3. **Set a decision deadline** — Open-ended escalations get deprioritized. A deadline creates urgency.
