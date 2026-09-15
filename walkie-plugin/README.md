# Walkie (Cursor / Grok Bot plugin)

Remote MCP connector for [Walkie](https://trywalkie.com) meetings. This folder is the Marketplace plugin: markdown, `mcp.json`, and an icon. No binaries.

- **URL:** `https://mcp.trywalkie.com/mcp`
- **Auth:** OAuth 2.0 (CIMD). Scope `meetings:read`.
- **Tools:** `search_meetings`, `get_meeting`, `list_meetings` (all read-only)
- **Plan:** Walkie Work or higher
- **Privacy:** https://trywalkie.com/en/privacy

The Claude Desktop `.mcpb` lives at the repo root, outside this plugin, so Marketplace review does not ingest a desktop binary.
