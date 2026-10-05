# Agent instructions

Shared rules for all AI coding agents (Claude Code, Codex, Gemini CLI).
This file is the single source of truth: `CLAUDE.md` and `GEMINI.md` only import it.
Edit rules here, never in those files.

## Language
- All code, comments, docstrings, commit messages and documentation MUST be written in **English**, unless the user explicitly requests another language for a specific item.

## Git
- Never add `Co-Authored-By:` trailers, "Generated with ..." lines or any other AI attribution to commits or pull requests.

## Agent resources
Before starting a task, check `.agents/`:

- `.agents/rules/` — mandatory rules. Read every file and follow them:
  - `general.md` — workflow, scope, communication.
  - `code-quality.md` — design principles, structure, naming, performance.
  - `safety-and-compatibility.md` — errors, security, resources, compatibility, destructive actions.
  - `domain-specific.md` — web, desktop, network, persistence, embedded.
  - `testing-and-verification.md` — tests, definition of done, failure limits.
  - `git.md` — commit conventions.
  - `tooling.md` — optional tools (caveman, graphify) when available.
- `.agents/skills/` — reusable procedures, one folder per skill with a `SKILL.md`. When a task matches a skill's description, read and follow that `SKILL.md`.
- `.agents/tools/` — scripts and configs (e.g. MCP servers) available to agents. Prefer them over ad-hoc commands.
- `.agents/prompts/` — reusable prompts the user can reference by name.

## Conventions
- Put documentation in `docs/`, not the repo root.
