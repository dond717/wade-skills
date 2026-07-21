# Zapier CEO Copilot: Shareable Skills

Three of the agent "skills" Wade Foster (Co-Founder & CEO, Zapier) demoed during his Running Remote 2026 fireside chat, cleaned up into general-purpose versions you can drop into your own AI setup.

A "skill" here is just a Markdown file that tells an AI agent (Cursor, Claude Code, Claude Projects, a custom GPT, etc.) how to run a specific workflow. Each one is written to be tool-agnostic: wherever the original relied on a specific tool, these versions use a generic placeholder like `[YOUR MEETING NOTES TOOL]` that you fill in once.

## The Three Skills

| Skill | What it does |
|-------|--------------|
| [`war-council/SKILL.md`](skills/war-council/SKILL.md) | Convenes a panel of opinionated expert personas (ruthless CFO, contrarian board member, customer obsessive, plus experts generated for your specific problem) to stress-test a decision and return a ranked, bet-weighted recommendation. |
| [`meeting-follow-up-pipeline/SKILL.md`](skills/meeting-follow-up-pipeline/SKILL.md) | Turns a finished meeting into a debrief, decisions, action items, ready-to-send follow-up drafts, and proposed writebacks into your task/CRM systems. |
| [`exec-weekly-agenda-generator/SKILL.md`](skills/exec-weekly-agenda-generator/SKILL.md) | Sweeps your week across meetings, chat, email, and calendar, then produces a forced-ranked list of 5-10 topics worth the leadership team's time. |

## How to Use Them

**In Claude Code:** install as a plugin — `claude plugin marketplace add zapier/marketplace` then `claude plugin install wade-skills@zapier`. All three skills become available automatically.

**In OpenAI Codex:** `codex plugin marketplace add zapier/marketplace` then `codex plugin add wade-skills@zapier`. Or open the in-CLI picker with `/plugins` and toggle it on.

**In GitHub Copilot CLI:** `copilot plugin marketplace add zapier/marketplace` then `copilot plugin install wade-skills@zapier`.

**In Cursor or Claude Code (manual):** drop a skill's folder into `.cursor/skills/` (Cursor) or `.claude/skills/` (Claude Code). The YAML frontmatter at the top of each file (`name` + `description`) is what tells the agent when to invoke it automatically. You can also just paste the file contents into a chat and say "follow this."

**In Claude Projects / a custom GPT / any chatbot:** paste the skill file into the system prompt or project knowledge. Then trigger it with the phrases listed under "When to Use."

**Fill in the placeholders first.** Each file has a short "Setup" section listing the `[BRACKETED]` placeholders (your meeting-notes tool, your email, your CRM, your leadership team roster, etc.). Set those once and the skill runs against your stack.

## A Note on Design

These work because of a few principles, not because of any specific vendor:

1. **Personas with flaws give better critiques than generic advisors.** The War Council members have backstories that include failures on purpose.
2. **Every output must trace to a real source.** The agenda generator refuses to include a topic it can't tie to an actual meeting, thread, or email. No generic "review metrics" filler.
3. **Propose, don't auto-execute.** The follow-up pipeline drafts and proposes writebacks but asks before sending or writing anything.
4. **Force ranking beats completeness.** Five strong items beat ten mediocre ones.

## License

Shared with the Running Remote community and released by Zapier, Inc. under the MIT License. See [LICENSE](LICENSE) for the license and [NOTICE](NOTICE) for trademark, third-party, and use terms. Review [NOTICE](NOTICE) before use.

This repo is shared as-is. We're not accepting external contributions.
