# /context-update — Update Context

Help a team member update their personal context entry.

If `$ARGUMENTS` is provided, treat it as the team member's name.

## Approach
1. Read `context/members/_template.md` as schema
2. Read existing `context/members/[name].md` if present
3. Ask for changes in the **Current** section (Focus, Actions, Blockers)
4. Write the updated file to `context/members/[name].md`
5. Update the corresponding row in `context/members/team.md`

## Notes
- Profile fields (MBTI, CliftonStrengths, Skills, Working Style) only change on explicit request
- Only the **Current** section is updated during a regular update
- Ask for the name if `$ARGUMENTS` is empty
