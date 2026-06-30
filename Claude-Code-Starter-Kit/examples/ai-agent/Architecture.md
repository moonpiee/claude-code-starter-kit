# Overview

The system combines a planning agent with repository tools and a simple task state model so it can turn requests into structured work.

# Folder Structure

```text
agent/
  planner/
  tools/
  memory/
  api/
```

# Backend

The agent interprets requests, plans steps, and uses repository tools to inspect code or files.

# Frontend

A minimal interface shows the task plan, current status, and suggested next actions.

# Database

A lightweight store tracks tasks, context, and agent decisions.

# APIs

- `POST /tasks`
- `GET /tasks/{id}`
- `POST /tasks/{id}/resume`

# External Services

- LLM provider
- Repository access layer
- Optional issue tracker integration

# Deployment

Containerized service with secure credentials and tool permissions.

# Future Scaling

Introduce multi-agent coordination and a stronger memory layer as the workflow matures.

# Key Decisions

### Date

2026-07-01

### Decision

Use a planning-first agent architecture that keeps the plan visible to the user.

### Reason

Visible planning improves trust and makes agent behavior easier to review.

### Tradeoffs

The workflow is slightly more verbose than a fully autonomous approach.

### Alternatives

- Fully autonomous execution with minimal user interaction
- A rules-based task manager with no AI planning layer

### Status

Accepted
