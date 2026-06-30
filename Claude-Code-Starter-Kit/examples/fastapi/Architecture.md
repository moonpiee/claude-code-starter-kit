# Overview

The backend uses FastAPI to ingest receipts, run OCR and categorization, and expose reporting endpoints.

# Folder Structure

```text
app/
  api/
  services/
  models/
  db/
```

# Backend

FastAPI handles routes and domain logic. Background workers process uploaded files asynchronously.

# Frontend

A simple admin dashboard is planned later; the first version focuses on API reliability.

# Database

PostgreSQL stores users, receipts, categories, and reports.

# APIs

- `POST /receipts`
- `GET /reports/{week}`
- `POST /categories/refresh`

# External Services

- OCR provider
- LLM provider for classification

# Deployment

Docker containers deployed behind a managed load balancer.

# Future Scaling

Introduce queue-based processing and read replicas as usage grows.

# Key Decisions

### Date

2026-07-01

### Decision

Use FastAPI and PostgreSQL for the MVP.

### Reason

They provide a strong balance of speed, reliability, and developer familiarity.

### Tradeoffs

The stack is slightly more complex than a simple script-based prototype.

### Alternatives

- Flask for a lighter web layer
- SQLite for faster startup

### Status

Accepted
