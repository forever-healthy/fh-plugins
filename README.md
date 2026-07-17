![Version 0.2.0](https://img.shields.io/badge/Version-0.2.0-green.svg)
[![Forever Healthy](https://img.shields.io/badge/(c)_2026-Forever_Healthy-573D7D.svg)](https://forever-healthy.org)

# Forever Healthy — Plugin Marketplace

An [Anthropic style plugin marketplace](https://docs.claude.com/en/docs/claude-code/plugins) for compatible environments (Claude Desktop, Claude Code, Grok Build, ...) by [Forever Healthy](https://forever-healthy.org).


## Plugins

For detailed instructions on the Evipedia plugins, see [https://evipedia.ai/integration](https://evipedia.ai/integration#evipedia-plugin)

### `evipedia`

Connects to the **Evipedia MCP server** running locally and bundles a `/demo` skill.

* **MCP tools** — search Evipedia reviews, read full reviews and their conclusions, and suggest new interventions, all against live [evipedia.ai](https://evipedia.ai) data. The server runs over stdio via `npx -y evipedia-mcp@latest` (requires Node.js).
* **`/demo` skill** — smoke-tests the connection by walking through the read tools against live data.

See [`evipedia/`](./evipedia) for the plugin manifest and its bundled MCP config.

### `evipedia-remote`

Same MCP tools and `/demo` skill as `evipedia`, but connects to the **hosted Evipedia MCP server** at [`https://mcp.evipedia.ai/mcp`](https://mcp.evipedia.ai/) over HTTP — no local Node.js install needed.

See [`evipedia-remote/`](./evipedia-remote) for the plugin manifest and its bundled MCP config.

The MCP server is maintained at [forever-healthy/evipedia-mcp](https://github.com/forever-healthy/evipedia-mcp) and published to npm as [`evipedia-mcp`](https://www.npmjs.com/package/evipedia-mcp).

## License

[MIT](./LICENSE) © Forever Healthy Foundation
