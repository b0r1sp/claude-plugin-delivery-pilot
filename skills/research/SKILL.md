---
name: research
description: Research and analyze a topic from a delivery or professional perspective. Use when asked to research, investigate, analyze, "what are best practices for", "compare options for", or "find out about". Adapts automatically to the active role if one is set via /delivery-pilot:role.
argument-hint: "[topic or question]"
---

# /delivery-pilot:research

> If tools are connected, see [CONNECTORS.md](../../CONNECTORS.md).

Targeted research and structured analysis. Automatically adapts perspective, questions, and output style to the **active role** (see **/delivery-pilot:role**).

## Usage

```
/delivery-pilot:research $ARGUMENTS
```

## Active Role

First, check `context/roles/active-role.md`:
- If a role is active, read `context/roles/[name].md`
- Apply that role's perspective, typical questions, frameworks, and output style
- Mention the active role at the top of the output

## Output

```markdown
**Research:** [Topic]
**Date:** [today]
**Role:** [active role, or "none"]

### Question
[Precise question to be answered]

### Context
[Why is this relevant? What problem needs to be solved?]

### Findings

| Aspect | Insight | Source / Basis |
|--------|---------|----------------|

### Comparison / Options (if applicable)

| Option | Pros | Cons | Recommendation |
|--------|------|------|----------------|

### Recommendation
[Clear recommendation with rationale]

### Open Questions
-
```

## If Connectors Available

If **~~knowledge base** is connected:
- Search internal documentation before going to general knowledge
- Surface existing decisions and past research

## Tips

1. **Activate a role first** — `/delivery-pilot:role it-consultant` before `/delivery-pilot:research cloud migration` gives a fundamentally different and more useful result.
2. **Quick Look vs. Deep Dive** — Say which one you want. Quick Look = key insights in minutes. Deep Dive = comprehensive analysis.
3. **Flag uncertainty** — If something can't be verified, say so rather than filling the gap with plausible-sounding content.
