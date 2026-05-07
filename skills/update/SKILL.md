---
name: update
description: Write a concise stakeholder update or project communication. Use when asked to draft an update, "message to stakeholders", "management update", "client update", or "project communication".
argument-hint: "[project name or target audience, e.g. 'Management' or 'Client']"
---

# /delivery-pilot:update

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Draft a clear, professional stakeholder update. See **/delivery-pilot:status** for the full project health picture and **/delivery-pilot:reporting** for formal periodic reports.

## Usage

```
/delivery-pilot:update $ARGUMENTS
```

## Output

```markdown
**Project Update – [Date]**
**To:** [Audience]
**From:** Delivery Lead

---

**Overall Status:** 🟢 On Track / 🟡 At Risk / 🔴 Off Track

**Highlights this week:**
-

**Risks & Mitigations:**
-

**Next Steps:**
-

**Decisions needed:**
- [ ]
```

## If Connectors Available

If **~~email** is connected:
- Draft the update as an email ready to send
- Pull recipient list from project contacts

If **~~chat** is connected:
- Format and post the update to the relevant channel

## Tips

1. **Positives first, then risks** — Lead with progress before problems.
2. **Make decisions easy** — For each decision needed, provide context and a recommendation.
3. **Less is more** — If they need to scroll, they won't read it. Cut ruthlessly.
