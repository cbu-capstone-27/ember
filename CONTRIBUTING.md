# Contributing to Ember

> Stub. Expand as tooling and conventions solidify. Jira: EMBER-28.

## Before you start

- Every change maps to a Jira ticket on the [EMBER board](https://ember-capstone.atlassian.net/browse/EMBER). If there is no ticket, create one first.
- Read `docs/working-agreement.md` and skim `docs/adr/` for decisions already made.

## Workflow

1. Branch from `develop`: `feature/EMBER-<n>-<short-slug>`.
2. Make your change. Keep PRs small and single-purpose.
3. Open a PR into `develop`. Fill out the template completely; the Jira key is mandatory and should also lead the PR title (`EMBER-<n>: ...`).
4. CI must be green (`ci-ok`) and required reviewers (see `.github/CODEOWNERS`) must approve.
5. Squash-merge unless there is a reason to preserve history.

`main` receives merges from `develop` only, for releases. Hotfixes branch from `main` as `hotfix/EMBER-<n>-<slug>` and are merged back to both `main` and `develop`.

## Repository layout

See the "Repository layout" section of `README.md`. In short: apps in `apps/`, background services in `services/`, shared code in `packages/` (only once a second consumer exists), local infra in `infra/`, decisions in `docs/adr/`.

## Architecture decisions

Anything hard to reverse or cross-cutting gets an ADR in `docs/adr/`. See `docs/adr/0000-use-adrs.md` for the format.

## Local setup

```sh
cp .env.example .env
docker compose -f infra/docker-compose.yml --env-file .env up -d
```

Per-app setup instructions live in each app's README once code exists.
