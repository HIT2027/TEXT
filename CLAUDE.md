# CLAUDE.md

This file provides guidance for AI assistants (Claude Code and similar tools) working in this repository.

## Repository Overview

**Repository**: HIT2027/TEXT  
**Status**: Initial setup — no application code exists yet.  
**Current branch convention**: Feature work happens on `claude/<description>` branches; merge targets `main`.

The repository was initialized with a single empty `.gitkeep` commit. This CLAUDE.md is the first substantive file.

---

## Repository Structure

```
TEXT/
├── CLAUDE.md          ← This file
└── .gitkeep           ← Placeholder from initialization
```

As the project grows, update this section to reflect the actual layout.

---

## Git Workflow

- **Default branch**: `main`
- **Feature branches**: `claude/<short-description>` (AI-driven) or `feat/<short-description>` (human-driven)
- Always develop on a feature branch; never commit directly to `main`.
- Commit messages should be concise and imperative: `Add login endpoint`, `Fix null check in parser`.
- Push with `git push -u origin <branch-name>`.

---

## Development Setup

> This section should be updated once the project stack is chosen.

Until a stack is defined, there are no install steps, build commands, or environment variables to document.

---

## Testing

> No test framework has been configured yet.

When tests are added, document here:
- How to run the full test suite
- How to run a single test file
- Coverage thresholds, if any

---

## Linting & Formatting

> No linter or formatter has been configured yet.

When tooling is added (ESLint, Prettier, Ruff, Black, etc.), document the commands here and note whether they run as pre-commit hooks or in CI.

---

## CI/CD

> No CI/CD pipelines exist yet.

When GitHub Actions or another CI system is introduced, document:
- Which workflows run on PR open/push
- Required checks before merge
- Deployment targets and triggers

---

## Conventions for AI Assistants

- **Read before editing**: Always read a file with the Read tool before modifying it.
- **Minimal changes**: Make only the changes required by the task — no unsolicited refactors or cleanups.
- **No speculative comments**: Do not add comments that explain what code does; only add comments for non-obvious *why* reasoning.
- **No new files without cause**: Prefer editing existing files. Create new files only when the task explicitly requires them.
- **Branch discipline**: All work goes on the designated feature branch. Never push to `main` directly.
- **Commit before pushing**: Stage and commit changes with a clear message before pushing.
- **Security**: Never commit secrets, credentials, or `.env` files. Check for accidental secret exposure before committing.
- **Update this file**: When new tooling, structure, or conventions are introduced, update the relevant section of this CLAUDE.md.

---

## Key Files to Update as the Project Grows

| File | Purpose |
|------|---------|
| `CLAUDE.md` | AI assistant guidance (this file) |
| `README.md` | Human-facing project overview |
| `.github/workflows/` | CI/CD pipeline definitions |
| `.gitignore` | Files to exclude from version control |
| Package/dependency manifest | `package.json`, `pyproject.toml`, `Cargo.toml`, etc. |

---

*Last updated: 2026-06-03 — initial creation on empty repository.*
