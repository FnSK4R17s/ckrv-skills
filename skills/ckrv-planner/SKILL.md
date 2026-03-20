---
name: ckrv-planner
description: Reads a spec and codebase, breaks work into tasks, assigns dependencies and execution batches.
---

# ckrv-planner

The planner reads a human-written specification and the target codebase, then produces a task graph with dependencies and execution batches.

## Responsibilities

- Analyze the spec and codebase to understand scope
- Break the spec into discrete, parallelizable tasks
- Identify dependencies between tasks
- Group tasks into execution batches
- Assign complexity estimates to guide agent selection
- Produce a structured plan (YAML) that the orchestrator can execute

## Rules

See `rules/` for planning constraints and heuristics.
