# Codex Setup

This fork keeps Mads Lorentzen's job-search framework and adds a Codex entry point. Open this folder as a Codex project and use the repository skill at `.codex/skills/job-search/SKILL.md`.

## Start

Ask Codex to `Use $job-search to set up my candidate profile`, `Use $job-search to search for software engineering jobs`, or `Use $job-search to apply to this posting: <URL or text>`.

The skill covers setup, search, ranking, applications, outcomes, interview preparation, gap analysis, reports, templates, portals, and optional connected-service sync. It reads only the relevant upstream workflow for each request. The upstream `.claude/` directory remains intact so future upstream changes can be compared.

## Personal data

This GitHub fork is public. The upstream setup process writes personal details into tracked `CLAUDE.md` and `.claude/skills/` files. The Codex workflow instead reads `../resume-system/master_experience.md` when that sibling repo is present, and writes any confirmed additions to ignored `private/candidate.md`. Keep generated application files in the ignored paths described in `AGENTS.md`.

Before pushing, inspect `git status` and `git diff --cached` for contact details, private notes, and application materials. The Codex skill never needs to commit those files.

## Dependencies

The original PDF path needs Python 3.10+, LaTeX (`lualatex` and `xelatex`), and a PDF text extractor (`pypdf` or `pdftotext`). Job portal CLIs use Bun. Codex can still analyze a posting and draft source files when an optional tool is missing, but should state which output checks were skipped. Do not run upstream `/setup` in Claude Code on this public fork because it populates tracked files.

## Upstream

`origin` points at this fork and `upstream` points at `MadsLorentzen/ai-job-search`. Merge upstream changes deliberately, because their instructions and tests may still assume Claude Code.
