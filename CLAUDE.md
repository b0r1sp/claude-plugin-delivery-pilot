# Claude Plugin – Delivery Pilot

This plugin supports Delivery Leads and project professionals in their daily work.
All commands are organized in three dimensions:

| Dimension         | Commands                                                        |
|-------------------|-----------------------------------------------------------------|
| **Data**          | `/status`, `/risks`, `/timeline`                                |
| **Tools**         | `/estimate`, `/research`, `/context-update`                     |
| **Collaboration** | `/agile-standup`, `/agile-retrospective`, `/update`, `/escalate`, `/handover`, `/reporting` |

## General
- Language: English (unless specified otherwise)
- Tone: professional, concise
- Templates located under `templates/`

## Context Layer

All commands read from `context/` first when available.

```
context/
├── members/        # Profile + current status per team member
├── project/        # Decisions, actions, artifacts
├── mails/          # Relevant mails (summarized)
├── chats/          # Relevant chat threads
└── files/          # Referenced documents
```

- New team members: copy `context/members/_template.md` → `[name].md`
- Weekly update: `/context-update [name]`
- File conventions: see `_readme.md` in each directory
