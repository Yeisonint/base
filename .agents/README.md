# .agents

Tool-agnostic resources for AI coding agents. Referenced from `AGENTS.md`.

| Folder | Content | Format |
|---|---|---|
| `rules/` | Mandatory rules (style, architecture, git, testing). | One Markdown file per topic. |
| `skills/` | Reusable procedures the agent applies when relevant. | `skills/<name>/SKILL.md` with `name` and `description` frontmatter, plus optional supporting files. |
| `tools/` | Helper scripts and MCP server configs. | Any script; document usage at the top of each file. |
| `prompts/` | Reusable prompts / task templates. | One Markdown file per prompt. |
