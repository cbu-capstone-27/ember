# apps/mcp

MCP (Model Context Protocol) server that exposes the Ember knowledge graph to AI coding tools.

## Status

Stub. No tool implementations yet. Tool surface, transport, and auth will each land under their own Jira ticket.

## Conventions

- This package is the only place MCP protocol handling lives.
- Graph access goes through shared code in `packages/` once a second consumer exists; until then it may live here.
