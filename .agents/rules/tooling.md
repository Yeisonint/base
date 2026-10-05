# Optional agent tooling

Use these tools only when they are available in the current agent environment. If a tool is not installed or not supported, skip it silently and continue normally.

## caveman
- If the `caveman` skill/plugin is available, use it at the **ultra** level for all responses (`/caveman ultra`).
- Code, commit messages, pull requests, documentation and security warnings are always written normally, never in caveman style.

## graphify
- If the `graphify` skill or CLI is available, use it for questions about the codebase, architecture or file relationships.
- If `graphify-out/graph.json` exists, query the graph first (`graphify query "<question>"`, `graphify path "<A>" "<B>"`, `graphify explain "<node>"`) before searching files manually.
- After significant code changes, update the graph incrementally (`/graphify . --update`) when a graph already exists.
- Do not build a full graph from scratch without asking the user first; it can be slow and costly on large repositories.
