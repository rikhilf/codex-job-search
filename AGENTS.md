---
framework_version: 1.0.0
---

# Agent Guidelines: AI Job Search (Codex fork)

Use the original procedures in `.claude/commands/` and `.claude/skills/` as the workflow specification. For Codex, start with `.codex/skills/job-search/SKILL.md`; it maps the Claude-specific commands and tools to Codex. The portal search skills in `.agents/skills/` remain available.

## Candidate profile and privacy

This fork is public. Do not populate tracked `CLAUDE.md` or `.claude/skills/**` with personal data. Use ignored `private/candidate.md` for confirmed profile facts and preferences. The sibling `../resume-system/master_experience.md`, when present, can supply source facts; do not copy it into the fork. Treat its `PRIVATE:` notes as strategy and `VERIFY:` facts as unconfirmed. Never use upstream example identity or credentials as candidate facts.

## Output

Keep the original `/apply` sequence: evaluate fit, ask whether to draft, create the CV and cover letter, review, compile and inspect the PDFs, run the final checks, and record the draft. Follow the original two-page CV and one-page cover-letter templates unless the user requests a different format. For technical roles, select only supported experience and never invent facts. Do not submit applications or send messages without explicit authorization.
