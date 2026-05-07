# Claude Plugin – Delivery Pilot

This plugin supports Delivery Leads and project professionals in their daily work.
All skills are organized in three dimensions:

| Dimension         | Skills                                                                                                          |
|-------------------|-----------------------------------------------------------------------------------------------------------------|
| **Data**          | `/delivery-pilot:status`, `/delivery-pilot:risks`, `/delivery-pilot:timeline`                                   |
| **Tools**         | `/delivery-pilot:estimate`, `/delivery-pilot:research`, `/delivery-pilot:context-update`, `/delivery-pilot:role` |
| **Collaboration** | `/delivery-pilot:agile-standup`, `/delivery-pilot:agile-retrospective`, `/delivery-pilot:update`, `/delivery-pilot:escalate`, `/delivery-pilot:handover`, `/delivery-pilot:reporting` |

## General
- Language: English (unless specified otherwise)
- Tone: professional, concise

## Context Layer

All skills read from `context/` first when available.

```
context/
├── members/        # Profile + current status per team member
├── project/        # Decisions, actions, artifacts
├── roles/          # Role definitions + active-role state
├── mails/          # Relevant mails (summarized)
├── chats/          # Relevant chat threads
└── files/          # Referenced documents
```

- New team members: copy `context/members/_template.md` → `[name].md`
- Weekly update: `/delivery-pilot:context-update [name]`
- Activate a role: `/delivery-pilot:role [role-name]`
- Tool integrations: see `CONNECTORS.md`
