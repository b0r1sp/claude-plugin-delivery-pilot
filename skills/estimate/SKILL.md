---
name: estimate
description: Estimate effort for a feature, task, or epic using PERT analysis. Use when asked to estimate work, "how long will this take", "story points", "effort estimation", or when planning a sprint or release.
argument-hint: "[feature, task, or epic description]"
---

# /delivery-pilot:estimate

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Structured effort estimation using PERT (Program Evaluation and Review Technique). Use **/delivery-pilot:timeline** to place estimates on the project roadmap.

## Usage

```
/delivery-pilot:estimate $ARGUMENTS
```

## PERT Formula

```
Estimate = (Best + 4 × Most Likely + Worst) / 6
```

## Output

```markdown
**Estimate for:** [Name]

| Subtask | Best | Likely | Worst | PERT | Uncertainty |
|---------|------|--------|-------|------|-------------|
|         |      |        |       |      |             |
| **Total** |   |        |       |      |             |

**Unit:** Hours / Days
**Assumptions:**
-
**Risk buffer:** +X%
```

## If Connectors Available

If **~~project tracker** is connected:
- Pull similar past tasks and use actuals to calibrate estimates
- Create estimation tickets with PERT values attached

## Tips

1. **Break it down** — Estimates on large items are guesses. Estimates on small items are data.
2. **Document assumptions** — An estimate without assumptions is a promise. With assumptions, it's a forecast.
3. **Add a risk buffer** — 10–20% for known unknowns, more for novel work.
