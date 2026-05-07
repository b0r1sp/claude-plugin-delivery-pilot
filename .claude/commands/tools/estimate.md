# /estimate — Effort Estimation

Support the Delivery Lead with a structured effort estimation.

If `$ARGUMENTS` is provided, treat it as a feature, task, or epic.

## Approach
1. Break the task into subtasks
2. For each subtask: estimate Best Case / Most Likely / Worst Case (PERT)
3. Apply PERT formula: `(Best + 4×Most Likely + Worst) / 6`
4. Document assumptions and uncertainty factors

## Output Format

**Estimate for:** $ARGUMENTS

| Subtask | Best | Likely | Worst | PERT | Uncertainty |
|---------|------|--------|-------|------|-------------|
|         |      |        |       |      |             |
| **Total** |    |        |       |      |             |

**Unit:** Hours / Days (please specify when invoking)

**Assumptions:**
- 
**Risk buffer:** +X%

Ask for unit and context if not provided.
