# tartarus-mcp

> **This project has moved to [saluca-labs](https://github.com/saluca-labs).** This repo is now maintained at [`saluca-labs/tartarus-mcp`](https://github.com/saluca-labs/tartarus-mcp). Please update your remotes:
> ```bash
> git remote set-url origin https://github.com/saluca-labs/tartarus-mcp.git
> ```


Local-first MCP memory server. Persistent, searchable memory for any AI agent.

Powered by [@saluca/asphodel](https://www.npmjs.com/package/@saluca/asphodel). Zero cloud dependencies. SQLite-backed.

## Install

```bash
npx tartarus-mcp install
```

Automatically configures Claude Code, Cursor, and Windsurf.

## Manual setup

Add to your MCP settings:

```json
{
  "mcpServers": {
    "tartarus": {
      "command": "npx",
      "args": ["tartarus-mcp@latest"]
    }
  }
}
```

## Tools

| Tool | Description |
|------|-------------|
| `memory_remember` | Store a memory (topics auto-extracted) |
| `memory_recall` | Retrieve memories by topic |
| `memory_search` | Full-text search across all memories |
| `memory_forget` | Delete a memory by ID |
| `memory_list` | List recent memories |

## Config

```bash
TARTARUS_DB=/path/to/memory.db  # default: ~/.tartarus/memory.db
```

## Enterprise

Hash-chained audit trails, multi-tenant isolation, compliance controls, and team memory at [asphodel.ai](https://asphodel.ai).

## License

Apache 2.0 — [Saluca LLC](https://saluca.com)