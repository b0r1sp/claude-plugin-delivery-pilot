# Claude Plugin – Delivery Pilot

Claude Code plugin for delivery professionals. Commands for project management, collaboration, research, coaching, and role-based workflows.

## Structure

```
.claude/commands/
├── data/           # /status, /risks, /timeline
├── tools/          # /estimate, /research, /context-update
└── collaboration/  # /agile-standup, /agile-retrospective,
                    # /update, /escalate, /handover, /reporting

context/
├── members/        # Team profiles (MBTI, CliftonStrengths, Skills)
├── project/        # Decisions, actions, artifacts
├── mails/          # Relevant mails
├── chats/          # Relevant chat threads
└── files/          # Referenced documents
```

## Setup

1. Clone the repository
2. Start Claude Code from this directory
3. Create your profile: copy `context/members/_template.md` → `[name].md`
4. Fill in your profile and keep it current via `/context-update`

## Commands

| Command | Dimension | Description |
|---------|-----------|-------------|
| `/status` | Data | Create or update project status |
| `/risks` | Data | Manage risk register |
| `/timeline` | Data | Milestone overview |
| `/estimate` | Tools | Effort estimation (PERT) |
| `/research` | Tools | Research & analysis |
| `/context-update` | Tools | Update your context entry |
| `/agile-standup` | Collaboration | Prepare daily standup |
| `/agile-retrospective` | Collaboration | Sprint retrospective |
| `/update` | Collaboration | Write stakeholder update |
| `/escalate` | Collaboration | Formulate escalation |
| `/handover` | Collaboration | Create handover document |
| `/reporting` | Collaboration | Create report |
