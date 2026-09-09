# Walkie for MCP

Give Claude, Cursor, and any MCP client access to your recorded meetings —
search across everything you've said or heard, and pull any meeting's notes,
action items, participants, and speaker-labeled transcript.

[Walkie](https://trywalkie.com) records and transcribes your meetings on your
computer. This is its Model Context Protocol (MCP) connector.

## Install

### Claude Desktop (one click)
Download **[walkie.mcpb](./walkie.mcpb)** and open it in Claude Desktop
(**Settings → Extensions → Install**). It launches Walkie's local MCP server
automatically — no config needed, and it carries the Walkie icon.

### Any MCP client (command)
Point your client at Walkie's local server, e.g. for Claude Code or Cursor:
```
claude mcp add walkie -- /Applications/Walkie.app/Contents/MacOS/walkie --mcp-serve
```

### Remote (hosted, for web/mobile clients)
Connect over OAuth 2.0 to `https://mcp.trywalkie.com/mcp`.

## Requirements
- The **Walkie desktop app** (macOS/Windows) — the local server reads Walkie's
  on-device meeting database.
- A **Walkie Work plan** or higher.

## Tools
- **search_meetings** — find meetings by keyword across titles, notes, and transcripts.
- **get_meeting** — read one meeting's notes, action items, participants, and transcript.
- **list_meetings** — enumerate meetings as metadata (requires full archive access).

All three tools are **read-only**.

## Privacy
This connector runs on your computer and reads only your local Walkie data to
answer the requests your MCP client makes — it sends nothing anywhere itself.
Full policy: https://trywalkie.com/en/privacy

## License
MIT — see [LICENSE](./LICENSE).
