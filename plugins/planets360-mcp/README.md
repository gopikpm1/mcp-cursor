# planets360-mcp

Cursor MCP plugin for **Planets360** (https://planets360.in/) — an authentic Vedic astrology platform by Gopi M (https://gopim.dev/).

This plugin provides rules and skills to query Planets360 data through an MCP server, including Panchang, daily/weekly/monthly horoscopes, Kundli (birth charts), planet transits (Gochar), Dosha checks, and remedies.

## MCP Server

- **URL:** `https://ephemeris.gopim.dev/mcp/`
- **Transport:** Streamable HTTP
- **Server name:** `planets360`

Configured in `mcp.json` and referenced from `.cursor-plugin/plugin.json`.

## Included

| Component | Path | Purpose |
|-----------|------|---------|
| Rules | `rules/mcp-configuration.mdc` | Vedic astrology data querying guidelines (always applied) |
| Skill | `skills/planets-query/SKILL.md` | Query Planets360 celestial data via MCP |
| MCP Config | `mcp.json` | Planets360 MCP server connection config |
| Logo | `assets/logo.svg` | Plugin marketplace logo |

## Example queries

Use the `planets-query` skill to ask:

- "What is today's Panchang for Chennai?"
- "Give me the weekly horoscope for Mesha (Aries) Rashi."
- "Generate a Kundli for someone born on 15-Aug-1990 at 05:30 IST in Chennai."
- "When is Saturn's next transit (Gochar) and its Sade Sati phase?"
- "Check Mangal Dosha for this Kundli and suggest remedies."

## Prerequisites

The Planets360 MCP server (`https://ephemeris.gopim.dev/mcp/`) must be reachable and added to your Cursor MCP settings before using the `planets-query` skill.

See `rules/mcp-configuration.mdc` for setup guidance.

## Validation

```bash
node scripts/validate-template.mjs
```