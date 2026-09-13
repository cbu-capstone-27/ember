<!--
Thanks for the PR. Every section marked REQUIRED must be filled in.
PR title should start with the Jira key, e.g. "EMBER-28: Scaffold monorepo".
-->

## Jira key (REQUIRED)

EMBER-

<!-- Link is optional; the key is not. Example: EMBER-28 -->

## Scope tier (REQUIRED)

Pick exactly one. Must match the ticket's Jira label.

- [ ] `floor` - guaranteed for April 2027
- [ ] `drop-first` - targeted, cut first under pressure
- [ ] `not-at-launch` - explicitly out of April 2027 scope
- [ ] `coursework` - capstone deliverable
- [ ] `n/a` - repo hygiene / tooling with no product scope

## Summary

<!-- What changed and why, in a few sentences. Link ADRs if a decision was made. -->

## Test plan (REQUIRED)

<!--
How did you verify this? Commands run, manual steps, screenshots.
If there is nothing to test (docs-only), say so explicitly.
-->

- [ ] ...

## Checklist

- [ ] Title includes the Jira key
- [ ] Targets `develop` (or `main` only for release/hotfix)
- [ ] Docs / ADR updated if behaviour or a decision changed
- [ ] No secrets or credentials committed (`.env.example` only)
