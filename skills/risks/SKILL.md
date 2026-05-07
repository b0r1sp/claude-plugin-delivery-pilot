---
name: risks
description: Manage and update the project risk register. Use when identifying risks, updating existing risks, or when asked "what are the risks", "risk assessment", "risk register", "what could go wrong".
argument-hint: "[new risk description, or filter like 'high' / 'open']"
---

# /delivery-pilot:risks

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Manage the project risk register. See the **status** skill for overall project health and **timeline** for milestone-related risks.

## Usage

```
/delivery-pilot:risks $ARGUMENTS
```

## Risk Matrix

| | Low Impact | Medium Impact | High Impact |
|---|-----------|---------------|-------------|
| **High Likelihood** | Medium | High | Critical |
| **Medium Likelihood** | Low | Medium | High |
| **Low Likelihood** | Low | Low | Medium |

## Output

```markdown
| ID | Risk | L | I | Priority | Mitigation | Owner | Status |
|----|------|---|---|----------|------------|-------|--------|
| R1 |      |   |   |          |            |       | Open   |
```

**Legend:** L = Likelihood, I = Impact (H/M/L)
**Priority:** HH=Critical · HM/MH=High · MM=Medium · else=Low

## If Connectors Available

If **~~project tracker** is connected:
- Pull open issues and flagged blockers as candidate risks
- Link mitigations to existing tasks

If **~~ITSM** is connected:
- Create risk tickets and assign owners automatically

## Tips

1. **Focus on what's controllable** — Only log risks you can actually mitigate or monitor.
2. **Review weekly** — A stale risk register is worse than none. Pair with **/delivery-pilot:status**.
3. **One owner per risk** — Shared ownership means no ownership.
