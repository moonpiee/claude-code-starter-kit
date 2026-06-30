# Overview

The application uses a Next.js frontend with server-side APIs for ticket management and AI assistance.

# Folder Structure

```text
src/
  app/
  components/
  lib/
  api/
```

# Backend

A small API layer powers ticket lookup, profile data, and AI response suggestions.

# Frontend

The Next.js app includes an inbox, ticket details page, and profile views.

# Database

PostgreSQL stores users, tickets, customer metadata, and actions.

# APIs

- `GET /api/tickets`
- `GET /api/tickets/{id}`
- `POST /api/tickets/{id}/suggest`

# External Services

- Authentication provider
- AI completion service

# Deployment

Vercel for the frontend, plus managed API hosting and a relational database.

# Future Scaling

Introduce caching and a queue for background enrichment jobs as the ticket volume grows.

# Key Decisions

### Date

2026-07-01

### Decision

Use Next.js for the frontend and PostgreSQL for persistence.

### Reason

The product needs strong UX delivery and reliable structured data support.

### Tradeoffs

The stack introduces more setup complexity than a static site.

### Alternatives

- Plain React with a custom build pipeline
- A no-code internal tool for the MVP

### Status

Accepted
