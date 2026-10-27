# Planets360 MCP — Cursor Plugin

Cursor MCP plugin for **Planets360** (https://planets360.in/) — an authentic Vedic astrology platform by Gopi M (https://gopim.dev/).

This plugin provides rules and skills to query Planets360 data through an MCP server, including Panchang, daily/weekly/monthly horoscopes, Kundli (birth charts), planet transits (Gochar), Dosha checks, and remedies.

## MCP Server

- **URL:** `https://ephemeris.gopim.dev/mcp/`
- **Transport:** Streamable HTTP
- **Server name:** `planets360`

Configured in `plugins/planets360-mcp/mcp.json` and referenced from `plugins/planets360-mcp/.cursor-plugin/plugin.json`.

## Included

- `plugins/planets360-mcp/rules/mcp-configuration.mdc` — Vedic astrology data querying guidelines (always applied)
- `plugins/planets360-mcp/skills/planets-query/SKILL.md` — skill for querying Planets360 celestial data via MCP
- `plugins/planets360-mcp/mcp.json` — Planets360 MCP server connection config
- `plugins/planets360-mcp/assets/logo.svg` — plugin logo

## Prerequisites

The Planets360 MCP server (`https://ephemeris.gopim.dev/mcp/`) must be reachable and added to your Cursor MCP settings before using the `planets-query` skill.

See `plugins/planets360-mcp/rules/mcp-configuration.mdc` for setup guidance.

## Validation

```bash
node scripts/validate-template.mjs
```

Fix all reported errors before committing.
