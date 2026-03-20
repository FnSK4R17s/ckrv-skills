# ckrv-skills

Agent skills for [chakravarti-cli](https://github.com/FnSK4R17s/chakravarti-cli) — the open, transparent coding team.

## Skills

| Skill | Role | Description |
|-------|------|-------------|
| `ckrv-spec` | Spec | Generates, clarifies, and validates feature specifications from natural language descriptions |
| `ckrv-planner` | Planner | Reads a spec and codebase, breaks work into tasks, assigns dependencies and execution batches |
| `ckrv-developer` | Developer | Implements assigned tasks in an isolated git worktree. Writes code and tests |
| `ckrv-reviewer` | Reviewer | Reviews diffs against the spec. Catches bugs, style violations, and architectural drift |
| `ckrv-tester` | Tester | Runs existing tests. Writes new tests for generated code. Reports coverage |
| `ckrv-deployer` | Deployer | Deploys to Vercel and Cloudflare. Runs CI/CD checks. Verifies the build |

## Install

```bash
npx skills add FnSK4R17s/ckrv-skills
```

## Structure

Each skill follows a consistent structure:

```
skills/{skill-name}/
  SKILL.md          # Entry point with YAML frontmatter
  metadata.json     # Structured metadata (name, version, role)
  rules/            # Individual rule files
  resources/        # Scripts and supporting files
```

## License

MIT
