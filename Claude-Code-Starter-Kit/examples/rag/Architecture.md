# Overview

The system ingests internal documents, creates vector embeddings, and answers questions using a retrieval layer plus an LLM.

# Folder Structure

```text
app/
  ingest/
  retrieval/
  prompts/
  api/
```

# Backend

A document ingestion pipeline prepares content, while the retrieval service handles semantic search and grounding.

# Frontend

A lightweight chat interface lets employees ask questions and review citations.

# Database

A vector database stores embeddings and a relational store keeps metadata and user access logs.

# APIs

- `POST /ingest`
- `POST /query`
- `GET /documents`

# External Services

- Embedding provider
- LLM provider
- Document storage provider

# Deployment

Private cloud deployment with internal authentication and access control.

# Future Scaling

Separate indexing workers from query serving and add caching for frequent queries.

# Key Decisions

### Date

2026-07-01

### Decision

Use a vector database plus an LLM for retrieval and answer generation.

### Reason

The product needs grounded answers over a large internal document set.

### Tradeoffs

The architecture is more complex than a simple keyword search tool.

### Alternatives

- Rule-based FAQ search
- Pure keyword search with no embeddings

### Status

Accepted
