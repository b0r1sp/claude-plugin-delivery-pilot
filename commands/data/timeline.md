# /timeline — Milestone Overview

Create or update a milestone timeline for the project.

If `$ARGUMENTS` is provided, treat it as the project name, time range, or specific milestone.

## Tasks
- Capture milestones with date, owner and status
- Mark delays and dependencies
- Highlight critical path

## Output Format

**Project:** $ARGUMENTS

| Milestone | Planned | Forecast | Status | Owner | Dependency |
|-----------|---------|----------|--------|-------|------------|
|           |         |          | 🟢/🟡/🔴 |       |            |

**Status:** 🟢 On Track · 🟡 At Risk · 🔴 Delayed · ✅ Done

**Critical Path:**  
→ [Milestone 1] → [Milestone 2] → ...

Ask for missing data before finalizing the timeline.
