# Codex Runtime

The detailed procedures remain in `.claude/commands/` and `.claude/skills/`. Read the requested procedure as reference, then use tools actually available in this Codex session.

- `$ARGUMENTS` means the URL, posting, company, role, or options in the user's request. Claude slash-command syntax is not required.
- `Read`, `Glob`, `Grep`, `Edit`, `Write`, `Bash`, `WebFetch`, and `WebSearch` map to available Codex file, shell, and browsing tools. Do not assume a particular tool exists.
- A Claude `Agent` or `Task` reviewer maps to a bounded independent review with a subagent when available. Otherwise run a separate critical pass using the posting, source profile, and exact draft; record what was checked.
- A Claude interactive prompt maps to a concise question only when a missing fact blocks an accurate result.
- Do not rely on `.claude/settings.json`, Claude hooks, Claude MCP connectors, or auto-executed slash commands. Gmail and Notion operations require suitable available tools and user authorization.

The upstream profile paths are legacy defaults. Use `private/candidate.md` when present and `../resume-system/master_experience.md` when available. Never put personal data in tracked `CLAUDE.md` or `.claude/skills/**`. Keep profile and application outputs out of commits.

Before a resume is ready, check every claim, page count, visible layout, and extractable text when producing PDF. Honor a format explicitly requested by the user. The default is a one-page technical resume.
