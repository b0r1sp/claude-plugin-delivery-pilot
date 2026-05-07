---
name: reporting
description: Create a structured report for internal or external audiences. Use when asked to write a weekly report, monthly report, executive summary, or when presenting results to leadership or clients.
argument-hint: "[report type like 'weekly' or 'monthly', and project/area]"
---

# /delivery-pilot:reporting

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Create a polished periodic report. Combines data from **/delivery-pilot:status**, **/delivery-pilot:timeline**, and **/delivery-pilot:risks** into a complete narrative for leadership or clients.

## Usage

```
/delivery-pilot:reporting $ARGUMENTS
```

## Report Types

- **Weekly**: Short week-in-review (1 page)
- **Monthly**: Detailed progress report
- **Executive Summary**: Compact decision brief

## Output

```markdown
**[Report Type] – [Date]**
**Project / Area:**
**Created by:** Delivery Lead

---

### Summary
[2–3 sentences: What is the current status?]

### Progress

| Area | Last Period | Current | Trend |
|------|------------|---------|-------|
|      |            |         | ↑/→/↓ |

### KPIs

| KPI | Target | Actual | Status |
|-----|--------|--------|--------|
|     |        |        | 🟢/🟡/🔴 |

### Highlights
-

### Risks & Mitigations
-

### Outlook / Next Period
-
```

## If Connectors Available

If **~~project tracker** is connected:
- Pull KPIs, completed work, and upcoming milestones automatically

If **~~email** is connected:
- Draft the report as a ready-to-send email to stakeholders

If **~~office suite** is connected:
- Export the report as a formatted document

## Tips

1. **Start with the summary** — If leadership reads nothing else, they should understand the state from those 3 sentences.
2. **Trends matter more than snapshots** — Show direction (↑/→/↓), not just current state.
3. **Pair with /delivery-pilot:update** for lighter-weight interim communications between formal reports.
