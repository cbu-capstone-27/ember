# apps/web

Web frontend for Ember (graph browser, review queue, admin surface).

## Status

Stub. No application code yet. Framework choice and scaffold will land under their own Jira ticket.

## Conventions

- Owns only UI concerns. Shared logic that a second consumer needs moves to `packages/` (see `packages/README.md`).
- Do not add a build toolchain here until there is code that needs one.
