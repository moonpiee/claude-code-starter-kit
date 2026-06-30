# Project Goal

Build a RAG-powered internal knowledge assistant that helps employees answer policy and product questions using company documents.

# Success Criteria

- 80% of employee questions are answered without escalation
- Retrieval accuracy stays above 90% for policy queries
- Average answer latency stays under 3 seconds

# Constraints

- RAG pipeline
- Vector database
- Private deployment
- 8-week MVP timeline

---

# Project Overview

This example project is a private knowledge assistant for internal documents.

# Objectives

- Make internal documentation easier to search
- Ground answers in source material
- Improve response quality for repetitive employee questions

# Tech Stack

Python, vector database, embedding provider, and an LLM provider.

# Coding Standards

- Keep prompts deterministic and reviewable
- Cite all major answers to source documents
- Treat data privacy as a first-class concern

# Folder Structure

- `app/ingest` for document processing
- `app/retrieval` for search logic
- `app/api` for request handling

# Commands

- `python -m app.api`
- `pytest`

# Architecture Notes

The retrieval layer should always return evidence before the LLM generates a final answer.

# Current Sprint

- Finish ingestion and indexing flow
- Add citation rendering in the UI

# Known Constraints

- Internal documents may contain sensitive data
- Search quality depends on chunking and metadata quality

# Things Claude Should Always Remember

Ground every answer in the retrieved source material and never invent context.
Provide citations wherever possible (source of truth)
