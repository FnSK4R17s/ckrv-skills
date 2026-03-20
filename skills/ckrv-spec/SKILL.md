---
name: ckrv-spec
description: Generates, clarifies, and validates feature specifications from natural language descriptions. Produces structured spec.yaml, design docs, and task breakdowns.
---

# ckrv-spec

The spec skill helps users write high-quality feature specifications that agents can execute. It generates structured specs from natural language, resolves ambiguities interactively, produces technical design documents, and breaks specs into implementation tasks.

## Responsibilities

- Generate structured spec.yaml from a natural language feature description
- Produce user stories with priorities (P1-P5) and acceptance scenarios
- Identify functional, non-functional, and security requirements
- Define measurable success criteria
- Surface ambiguities as clarification questions with options
- Generate technical design documents mapped to spec requirements
- Break specs into discrete tasks with complexity ratings and model tier assignments
- Validate spec completeness and correctness

## Workflow

1. **Generate** — User provides a description, skill produces a structured spec with user stories, requirements, success criteria, and clarifications
2. **Clarify** — Resolve any ambiguities surfaced during generation
3. **Design** — Produce a technical design document from the spec, detecting the project's existing tech stack
4. **Tasks** — Break the spec into phased implementation tasks (Setup, Foundation, User Stories, Polish) with complexity, model tier, and risk ratings
5. **Validate** — Check spec completeness at any point

## Output Format

All outputs are structured YAML or markdown, version-controlled in `.specs/NNN-name/`:

```
.specs/NNN-name/
  spec.yaml           # The specification
  design.md           # Technical design document
  research.md         # Research notes template
  tasks.yaml          # Implementation task breakdown
```

## Rules

See `rules/` for spec generation constraints, validation criteria, and output format requirements.
