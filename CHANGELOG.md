# Forever Healthy Plugins — Change Log


### v0.2.0 — 2026-07-17

* New plugin **`evipedia-remote`** — connects to the hosted Evipedia MCP server at
  `https://mcp.evipedia.ai/mcp` over HTTP (no local Node.js needed). Same MCP tools
  and bundled `/demo` skill as `evipedia`; the two differ only in transport.


### v0.1.4 — 2026-07-17

* `/demo` skill: resync from evipedia-mcp — no content change; server version
  tracked to 0.1.26 (plugin manifest stamped accordingly)


### v0.1.3 — 2026-07-16

* `/demo` skill: resync from evipedia-mcp — tightened wording; tool-prefix
  handling condensed to "use the tools as named, whatever their prefix"


### v0.1.2 — 2026-07-16

* `/demo` skill: resync from evipedia-mcp (skill version scheme moved to semver)


### v0.1.1 — 2026-07-16

* `/demo` skill: recognize the evipedia MCP tools when reached over the Claude
  desktop / Cowork bridge (`mcp__remote-devices__plugin_evipedia_evipedia__*`),
  not only the direct `mcp__evipedia__*` form


### v0.1.0 — 2026-07-12

* Initial public marketplace structure
* Ships the `evipedia` plugin (Evipedia MCP server + `/demo` skill)
