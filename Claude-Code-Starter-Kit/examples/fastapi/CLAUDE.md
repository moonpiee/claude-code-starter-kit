# Project Goal

Build an AI expense tracker API that helps small teams categorize spending automatically.

# Success Criteria

- 50 active teams in the first month
- 90% of receipts are categorized correctly
- API response time stays under 800ms for common requests

# Constraints

- FastAPI
- PostgreSQL
- Docker
- 4-week MVP timeline

---

# Project Overview

This example project is a FastAPI service for automated expense tracking.

# Objectives

- Accept receipt uploads reliably
- Classify expenses using AI
- Deliver readable summaries to finance teams

# Tech Stack

FastAPI, PostgreSQL, Docker, Python, and an OCR provider.

# Coding Standards

- Keep endpoints small and clearly named
- Validate input aggressively
- Write tests for business logic

# Folder Structure

- `app/api` for routes
- `app/services` for OCR and classification logic
- `app/db` for persistence

# Commands

- `uvicorn app.main:app --reload`
- `pytest`

# Architecture Notes

Treat document processing as async work to keep the API responsive.

# Current Sprint

- Add OCR integrations
- Implement report generation

# Known Constraints

- MVP budget is limited
- External service latency must be handled gracefully

# Things Claude Should Always Remember

Favor a clear API contract and reliable background processing.
