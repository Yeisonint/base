# Base Template

Minimal starting point for any project developed with AI coding agents
(Claude Code, Codex, Gemini CLI).

```
├── .agents/
│   ├── rules/      # Mandatory rules for agents
│   ├── skills/     # Reusable procedures (SKILL.md per folder)
│   ├── tools/      # Helper scripts / MCP configs
│   └── prompts/    # Reusable prompts
├── docs/           # Documentation
├── AGENTS.md       # Single source of truth for agent instructions
├── CLAUDE.md       # Imports AGENTS.md
└── GEMINI.md       # Imports AGENTS.md
```

Add your stack (web framework, backend, etc.) on top of this.
