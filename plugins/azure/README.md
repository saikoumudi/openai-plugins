# Azure Plugin

This plugin provides Microsoft Azure cloud workflows in
`plugins/azure`.

It includes the following skills:

- `appinsights-instrumentation`
- `azure-ai`
- `azure-aigateway`
- `azure-cloud-migrate`
- `azure-compliance`
- `azure-compute`
- `azure-cost`
- `azure-deploy`
- `azure-diagnostics`
- `azure-enterprise-infra-planner`
- `azure-hosted-copilot-sdk`
- `azure-kubernetes`
- `azure-kusto`
- `azure-messaging`
- `azure-prepare`
- `azure-quotas`
- `azure-rbac`
- `azure-resource-lookup`
- `azure-resource-visualizer`
- `azure-storage`
- `azure-upgrade`
- `azure-validate`
- `entra-app-registration`
- `microsoft-foundry`

## Plugin Structure

The plugin lives at:

- `plugins/azure/`

with this layout:

- `.codex-plugin/plugin.json`
  - required plugin manifest
  - defines plugin metadata, version, and entry points for Codex

- `.mcp.json`
  - MCP server configuration
  - connects Codex to the Azure MCP and Context7 tools used by the bundled skills

- `agents/`
  - plugin-level agent metadata
  - includes `agents/openai.yaml` for the OpenAI surface

- `skills/`
  - the skill payload
  - each skill follows the standard structure (`SKILL.md`, `references/`, `assets/`)

- `assets/`
  - plugin-level icons and static resources referenced by the manifest
  