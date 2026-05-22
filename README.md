# Dagger Realtime Chat

## What it does
Multi-user chat room with live messaging, user authentication, and searchable message history.

## Tech stack
- **Framework:** Remix (TypeScript)
- **Database:** PostgreSQL (full-text search with tsvector)
- **Realtime:** WebSockets (Server-Sent Events)
- **Pipeline:** Dagger (TypeScript)

## Key features
- GitHub OAuth authentication
- Live message delivery
- Search message history by keyword
- Docker service orchestration (Postgres + Redis session store)

## Run locally
```bash
dagger call run
```

## Pipeline details
- Spins up Postgres + Redis containers
- Runs database migrations
- Tests WebSocket connections
- Caches node_modules between runs

## Why Dagger?
Three services orchestrated in testable TypeScript. No docker-compose YAML. No GitHub lock-in.
