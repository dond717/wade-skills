# AGENTS.md

You're an AI agent (Claude Code, Cursor, Claude Projects, a custom GPT, ...) working with this repo, or being asked to install one of its skills.

## What this repo is

Three of the agent skills Wade Foster (Co-Founder & CEO, Zapier) demoed during his Running Remote 2026 fireside chat, cleaned up into general-purpose, tool-agnostic versions. Each skill is a single Markdown file with YAML frontmatter that tells an agent when and how to run a workflow.

This repo is shared as-is. **External contributions aren't accepted** — see [README.md](./README.md).

## The skills

| Skill | File | What it does |
|---|---|---|
| War Council | [war-council/SKILL.md](./war-council/SKILL.md) | Convenes a panel of expert personas to stress-test a decision and return a ranked, bet-weighted recommendation. |
| Meeting Follow-Up Pipeline | [meeting-follow-up-pipeline/SKILL.md](./meeting-follow-up-pipeline/SKILL.md) | Turns a finished meeting into a debrief, decisions, action items, and proposed writebacks. |
| Exec Weekly Agenda Generator | [exec-weekly-agenda-generator/SKILL.md](./exec-weekly-agenda-generator/SKILL.md) | Sweeps the week's meetings, chat, email, and calendar into a forced-ranked leadership agenda. |

## Installing a skill

- **Claude Code / Cursor**: copy the skill's folder into `.claude/skills/` or `.cursor/skills/`. The `name` and `description` in its frontmatter is what triggers automatic invocation.
- **Claude Projects / a custom GPT / any chatbot**: paste the `SKILL.md` contents into the system prompt or project knowledge, then trigger it with the phrases listed under that skill's "When to Use" section.

Each skill has `[BRACKETED]` placeholders under a "Setup" section. Fill those in once for the user's stack (meeting-notes tool, CRM, leadership roster, etc.) before running it for real.

## Before you act

Read [NOTICE](./NOTICE) — it covers trademark use, the "not an official product" disclaimer, AI-output caveats, and the user's responsibility for data privacy when a skill touches meeting transcripts, email, or CRM records. These skills are built to propose actions and drafts, not auto-execute — keep a human in the loop when running them.

## License

MIT — see [LICENSE](./LICENSE).
