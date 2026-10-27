# planets360-mcp

Cursor MCP plugin for **Planets360** (https://planets360.in/) — an authentic Vedic astrology platform.

This plugin provides rules and skills to query Planets360 data through an MCP server, including Panchang, daily/weekly/monthly horoscopes, Kundli (birth charts), planet transits (Gochar), Dosha checks, and remedies.

## MCP Server

- **URL:** `https://ephemeris.gopim.dev/mcp/`
- **Transport:** Streamable HTTP

Configured in `mcp.json` and referenced from `plugin.json`.

## Included

- `rules/`: Vedic astrology data querying guidelines for Panchang, horoscopes, Kundli, and transits
- `skills/planets-query/`: skill for querying Planets360 celestial data via MCP
- `mcp.json`: Planets360 MCP server connection config

## Prerequisites

The Planets360 MCP server (`https://ephemeris.gopim.dev/mcp/`) must be reachable and added to your Cursor MCP settings before using the `planets-query` skill.

See `rules/mcp-configuration.mdc` for setup guidance.