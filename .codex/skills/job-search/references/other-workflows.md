# Other Workflows

Use [runtime.md](runtime.md) for tool and profile mapping. Read only the selected upstream procedure. Slash-command names below are workflow labels, not installed Codex commands.

| Operation | Upstream procedure | Codex adaptation |
| --- | --- | --- |
| Search jobs | `.claude/skills/job-scraper/SKILL.md` | Use available portal skills in `.agents/skills/` and private technical-role filters. Save search state privately. |
| Rank jobs | `.claude/commands/rank.md` | Score against private profile and keep gaps visible. |
| Outcomes/follow-up | `.claude/commands/outcome.md` | Update ignored tracker/archive. Send only with explicit authorization. |
| Interview | `.claude/commands/interview.md` | Ground stories in profile and submitted materials. |
| Expand evidence | `.claude/commands/expand.md` | Require a supporting source artifact; store confirmed additions privately. |
| Upskill | `.claude/skills/upskill/SKILL.md` | Use repeated real posting gaps; distinguish learning goals from resume-ready skills. |
| HTML report | `.claude/commands/html-report.md` | Generate from local tracker; keep report ignored. |
| Add template | `.claude/commands/add-template.md` | Keep templates free of personal data; test one-page output. |
| Add portal | `.claude/commands/add-portal.md` | Inspect the portal and generated CLI before execution; respect access rules. |
| Gmail sync | `.claude/commands/gmail-sync.md` | Require an available authorized mail connector. Propose status changes before writing. |
| Notion sync | `.claude/commands/notion-sync.md` | Require an available authorized Notion connector. Share filenames, not private documents. |
| Reset | `.claude/commands/reset.md` | Show exact files and scope first; preserve tracked upstream references. |

Substitute `private/candidate.md` and `../resume-system/master_experience.md` for upstream candidate paths. Never execute destructive reset or external sync merely because it appears in an upstream procedure.
