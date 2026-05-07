---
name: handover
description: Create a structured handover document for a project or role. Use when transitioning a project, going on leave, changing teams, or when asked for a "handover", "transition document", or "knowledge transfer".
argument-hint: "[project name or handover context]"
---

# /delivery-pilot:handover

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Create a complete handover document. Combines context from **/delivery-pilot:status**, **/delivery-pilot:risks**, and **/delivery-pilot:timeline** into a single transition package.

## Usage

```
/delivery-pilot:handover $ARGUMENTS
```

## Output

```markdown
# Handover: [Project/Role]
**Date:** [today] | **From:** [Name] | **To:** [Name]

---

## 1. Project Overview
- Goal:
- Status:
- Timeline:

## 2. Open Tasks & Priorities

| Task | Priority | Deadline | Context |
|------|----------|----------|---------|
|      | H/M/L    |          |         |

## 3. Key Contacts

| Person | Role | Channel | Notes |
|--------|------|---------|-------|

## 4. Risks & Known Issues
-

## 5. Access & Resources
- Tools:
- Documents:
- Repos:

## 6. Key Decisions (Background)
-

## 7. Recommendations for the Successor
-
```

## If Connectors Available

If **~~knowledge base** is connected:
- Pull existing documentation, decisions, and architecture notes automatically
- Create the handover document directly in the knowledge base

If **~~project tracker** is connected:
- Import open tasks and in-progress items for section 2

If **~~file storage** is connected:
- List relevant documents and their locations for section 5

## Tips

1. **Write for someone who knows nothing** — The best handovers assume zero context.
2. **Background on decisions matters most** — The successor can find the tasks. They can't find the reasoning.
3. **Do a walkthrough** — A document alone is never enough. Schedule a 30-min call to walk through it.
