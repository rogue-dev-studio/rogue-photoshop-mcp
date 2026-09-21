# rogue-photoshop-mcp

**Rogue Development** MCP package for agents.

Rogue MCP bridge for Adobe Photoshop - raster editing and exports for agents

- Market: https://rogue-dev-studio.github.io/rogue-market-agent/

## Requirements

- Adobe Photoshop desktop installed
- Python 3.10+ and `uv` / `uvx` on PATH
- Optional: set `PS_VERSION` (default 2024)

## Install (Cursor)

Copy `cursor.mcp.fragment.json` into your Cursor MCP config, or merge:

```json
{
  "mcpServers": {
    "photoshop": {
      "command": "uvx",
      "args": [
        "--python",
        "3.10",
        "photoshop-mcp-server"
      ],
      "env": {
        "PS_VERSION": "2024"
      }
    }
  }
}
```

Then restart Cursor.

## License

MIT - Rogue Development. See `LICENSE` and `NOTICE`.
