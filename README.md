# Claude Plugin – Delivery Pilot

Claude Code plugin for delivery professionals. Commands for project management, collaboration, research, coaching, and role-based workflows.

## Installation

```bash
claude --plugin-dir ./claude-plugin-delivery-pilot
```

Or install via marketplace once published.

## Structure

```
.claude-plugin/
└── plugin.json         # Plugin manifest

commands/
├── data/               # status, risks, timeline
├── tools/              # estimate, research, context-update, role
└── collaboration/      # agile-standup, agile-retrospective,
                        # update, escalate, handover, reporting

context/
├── members/            # Team profiles (MBTI, CliftonStrengths, Skills)
├── project/            # Decisions, actions, artifacts
├── roles/              # Role definitions + active-role state
├── mails/              # Relevant mails
├── chats/              # Relevant chat threads
└── files/              # Referenced documents
```

## Setup

1. Clone the repository
2. Load the plugin: `claude --plugin-dir ./claude-plugin-delivery-pilot`
3. Create your profile: copy `context/members/_template.md` → `[name].md`
4. Fill in your profile and keep it current via `/delivery-pilot:context-update`

## Commands

| Command | Dimension | Description |
|---------|-----------|-------------|
| `/delivery-pilot:status` | Data | Create or update project status |
| `/delivery-pilot:risks` | Data | Manage risk register |
| `/delivery-pilot:timeline` | Data | Milestone overview |
| `/delivery-pilot:estimate` | Tools | Effort estimation (PERT) |
| `/delivery-pilot:research` | Tools | Research & analysis |
| `/delivery-pilot:context-update` | Tools | Update your context entry |
| `/delivery-pilot:role` | Tools | Activate a professional role |
| `/delivery-pilot:agile-standup` | Collaboration | Prepare daily standup |
| `/delivery-pilot:agile-retrospective` | Collaboration | Sprint retrospective |
| `/delivery-pilot:update` | Collaboration | Write stakeholder update |
| `/delivery-pilot:escalate` | Collaboration | Formulate escalation |
| `/delivery-pilot:handover` | Collaboration | Create handover document |
| `/delivery-pilot:reporting` | Collaboration | Create report |

## License

MIT © Boris Podzeit
