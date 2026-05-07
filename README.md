# Claude Plugin – Delivery Pilot

Claude Code plugin for delivery professionals. Skills for project management, collaboration, research, coaching, and role-based workflows.

## Installation

```bash
claude --plugin-dir ./claude-plugin-delivery-pilot
```

## Structure

```
.claude-plugin/
└── plugin.json         # Plugin manifest

skills/
├── status/             # Project status report
├── risks/              # Risk register
├── timeline/           # Milestone overview
├── estimate/           # Effort estimation (PERT)
├── research/           # Research & analysis
├── context-update/     # Update team member context
├── role/               # Activate professional role
├── agile-standup/      # Daily standup
├── agile-retrospective/ # Sprint retrospective
├── update/             # Stakeholder update
├── escalate/           # Escalation message
├── handover/           # Handover document
└── reporting/          # Periodic report

context/
├── members/            # Team profiles (MBTI, CliftonStrengths, Skills)
├── project/            # Decisions, actions, artifacts
├── roles/              # Role definitions + active-role state
├── mails/              # Relevant mails
├── chats/              # Relevant chat threads
└── files/              # Referenced documents
```

## Skills

| Skill | Dimension | Description |
|-------|-----------|-------------|
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

## Connectors

This plugin is tool-agnostic. See [CONNECTORS.md](CONNECTORS.md) for supported integrations (Slack, Teams, Jira, Atlassian, Notion, Microsoft 365, Google Workspace).

## License

MIT © Boris Podzeit
