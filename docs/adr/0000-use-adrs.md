# ADR 0000: Use Architecture Decision Records

- Status: Accepted
- Date: 2026-09-13
- Jira: EMBER-28

## Context

Ember is a capstone project with a rotating set of contributors and a design that will change over two semesters. Decisions made in chat, standups, or PR comments get lost. We need a lightweight, in-repo record of *why* things are the way they are, so new contributors (human or agent) can find the reasoning without asking.

## Decision

We will record significant architectural decisions as Architecture Decision Records (ADRs) in `docs/adr/`.

- One file per decision: `NNNN-short-kebab-title.md`, numbered sequentially, zero-padded to four digits.
- Each ADR has: Status, Date, Jira key, Context, Decision, Consequences.
- Status is one of `Proposed`, `Accepted`, `Deprecated`, `Superseded by ADR-NNNN`.
- ADRs are immutable once accepted. To change a decision, write a new ADR that supersedes the old one and update the old one's status line.
- ADRs land via normal PRs and follow the PR template (Jira key required).

"Significant" means: hard to reverse, affects more than one app/service/package, or something a future contributor would reasonably ask "why did we do this?" about.

## Consequences

- Small overhead per decision in exchange for a durable, searchable history.
- ADRs are a natural source for Ember's own knowledge graph later; keep them well-formed.
- Decisions that were not recorded are not considered settled.
