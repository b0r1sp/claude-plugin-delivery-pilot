# Connectors

## How tool references work

Skill files use `~~category` as a placeholder for whatever tool is connected in that category. For example, `~~project tracker` might mean Jira, Azure DevOps, Linear, or any other tool with an MCP server.

This plugin is **tool-agnostic** — skills describe workflows in terms of categories rather than specific products.

## Connectors for this plugin

| Category | Placeholder | Included servers | Other options |
|----------|-------------|-----------------|---------------|
| Calendar | `~~calendar` | Google Calendar | Microsoft 365 |
| Chat | `~~chat` | Slack | Microsoft Teams |
| Email | `~~email` | Gmail, Microsoft 365 | — |
| File storage | `~~file storage` | SharePoint | Google Drive |
| ITSM | `~~ITSM` | — | Jira Service Management, ServiceNow |
| Knowledge base | `~~knowledge base` | Confluence, Notion | Guru, Coda |
| Office suite | `~~office suite` | Microsoft 365 | Google Workspace |
| Project tracker | `~~project tracker` | Jira, Azure DevOps | Linear, ClickUp, Asana |
