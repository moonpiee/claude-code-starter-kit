# Project Goal

Build an AI agent that helps developers plan, break down, and execute software tasks from natural language requests.

# Success Criteria

- 80% of simple task requests are handled without manual intervention
- Average task decomposition time drops below 10 minutes
- Users report that the plan is useful in 90% of sessions

# Constraints

- AI agent workflow
- Tool access to repository and docs
- Secure handling of code context
- 6-week MVP timeline

---

# Project Overview

This example project is an AI task coordinator for software development workflows.

# Objectives

- Translate natural language requests into manageable steps
- Help engineers stay aligned while working through tasks
- Surface blockers and next actions clearly

# Tech Stack

Python, an LLM provider, repository tooling, and a lightweight task store.

# Coding Standards

- Keep agent behavior transparent and reviewable
- Prefer explicit tool use over hidden steps
- Fail gracefully when context is incomplete

# Folder Structure

- `agent/planner` for task decomposition
- `agent/tools` for repository actions
- `agent/api` for orchestrating requests

# Commands

- `python -m agent.api`
- `pytest`

# Architecture Notes

The agent should expose a clear plan and maintain a simple record of its reasoning steps.

# Current Sprint

- Add planning loop and status updates
- Improve tool selection accuracy

# Known Constraints

- Tool access must be restricted and auditable
- The system must remain understandable for human reviewers

# Things Claude Should Always Remember

The best agent experience is one that feels collaborative rather than mysterious.
