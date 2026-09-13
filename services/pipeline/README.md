# services/pipeline

Ingestion pipeline and job queue: pulls activity from GitHub, Jira, and Slack, extracts entities and relationships, and writes them to the Neo4j graph.

## Status

Stub. No ingestion or queue code yet. Connector, extraction, and queue work each land under their own Jira ticket.

## Conventions

- Long-running / background work lives here, not in `apps/`.
- Local infrastructure it depends on (Neo4j today) is defined in `infra/docker-compose.yml`.
