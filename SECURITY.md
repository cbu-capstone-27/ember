# Security Policy

> Stub. The team will finalize this under a follow-up ticket. Jira: EMBER-28.

## Supported versions

Ember is pre-release. There are no supported versions yet; only the `develop` and `main` branches receive fixes.

## Reporting a vulnerability

Please do **not** open a public issue for security problems.

- Preferred: use GitHub's private vulnerability reporting on this repository (Security tab -> "Report a vulnerability"), if enabled.
- Otherwise: contact the repository owner directly (see `.github/CODEOWNERS`).

Include what you found, how to reproduce it, and any impact you can assess. We will acknowledge within a reasonable time for a student project and keep you updated.

## Secrets

- Never commit credentials. Use `.env` (gitignored) locally and `.env.example` for documented placeholders.
- If a secret is committed, rotate it immediately and then remove it from history; treat it as compromised regardless.
