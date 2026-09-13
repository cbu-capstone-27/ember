# apps/cli

Command-line interface for Ember (local ingestion triggers, graph queries, developer utilities).

## Status

Stub. No application code yet. Language/runtime choice and scaffold will land under their own Jira ticket.

## Conventions

- Thin wrapper over shared logic. Anything the CLI needs that `apps/mcp` or `services/pipeline` also needs belongs in `packages/`.
