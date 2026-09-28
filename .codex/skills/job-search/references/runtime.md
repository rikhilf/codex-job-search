# Codex Runtime

The detailed procedures remain in `.claude/commands/` and `.claude/skills/`. Read the requested procedure as reference, then use tools actually available in this Codex session.

- `$ARGUMENTS` means the URL, posting, company, role, or options in the user's request. Claude slash-command syntax is not required.
- `Read`, `Glob`, `Grep`, `Edit`, `Write`, `Bash`, `WebFetch`, and `WebSearch` map to available Codex file, shell, and browsing tools. Do not assume a particular tool exists.
- A Claude `Agent` or `Task` reviewer maps to a bounded independent review with a subagent when available. Otherwise run a separate critical pass using the posting, source profile, and exact draft; record what was checked.
- Honor the upstream decision points, including its question after fit evaluation. Translate Claude's interactive prompt mechanism into a normal Codex question.
- Do not rely on `.claude/settings.json`, Claude hooks, Claude MCP connectors, or auto-executed slash commands. Gmail and Notion operations require suitable available tools and user authorization.

For candidate facts, substitute ignored `private/candidate.md` and, when available, `../resume-system/master_experience.md` for the upstream tracked profile files. Treat the latter's `PRIVATE:` notes as strategy and `VERIFY:` entries as unconfirmed. The tracked upstream profile/template files are workflow and layout references, not this candidate's identity. Keep profile and application outputs out of commits.

Do not inherit the example candidate's location, work authorization, relocation preference, languages, career goals, or tool usage. Ask when a missing preference is material to a decision. Do not present a template placeholder as a candidate fact.

Keep the upstream verification steps. The stock CV target is two pages and the cover letter one page, unless the user requests a different format.
