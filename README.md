![Version 0.1.4](https://img.shields.io/badge/Version-0.1.4-green.svg)
[![Forever Healthy](https://img.shields.io/badge/(c)_2026-Forever_Healthy-573D7D.svg)](https://forever-healthy.org)

# Forever Healthy — Claude Plugins

A [Claude Code plugin marketplace](https://docs.claude.com/en/docs/claude-code/plugins) from [Forever Healthy](https://forever-healthy.org), for working with [evipedia.ai](https://evipedia.ai) — our continuously-updated encyclopedia of evidence reviews on health & longevity interventions.

## Install

In Claude Code, add the marketplace and install the plugin:

```
/plugin marketplace add forever-healthy/fh-plugins
/plugin install evipedia@forever-healthy
```

## Plugins

### `evipedia`

Connects Claude to the **Evipedia MCP server** and bundles a `/demo` skill.

* **MCP tools** — search Evipedia reviews, read full reviews and their conclusions, and suggest new interventions, all against live [evipedia.ai](https://evipedia.ai) data. The server runs over stdio via `npx -y evipedia-mcp@latest` (requires Node.js).
* **`/demo` skill** — smoke-tests the connection by walking through the read tools against live data.

The MCP server is maintained at [forever-healthy/evipedia-mcp](https://github.com/forever-healthy/evipedia-mcp) and published to npm as [`evipedia-mcp`](https://www.npmjs.com/package/evipedia-mcp).

See [`evipedia/`](./evipedia) for the plugin manifest and its bundled MCP config.

## License

[MIT](./LICENSE) © Forever Healthy Foundation
