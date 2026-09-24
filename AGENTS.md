# AGENTS.md

You're an AI agent (Claude Code, Cursor, Claude Projects, a custom GPT, ...) working with this repo, or being asked to install one of its skills.

## What this repo is

Three of the agent skills Wade Foster (Co-Founder & CEO, Zapier) demoed during his Running Remote 2026 fireside chat, cleaned up into general-purpose, tool-agnostic versions. Each skill is a single Markdown file with YAML frontmatter that tells an agent when and how to run a workflow.

This repo is shared as-is. **External contributions aren't accepted** — see [README.md](./README.md).

## The skills

| Skill | File | What it does |
|---|---|---|
| War Council | [war-council/SKILL.md](./skills/war-council/SKILL.md) | Convenes a panel of expert personas to stress-test a decision and return a ranked, bet-weighted recommendation. |
| Meeting Follow-Up Pipeline | [meeting-follow-up-pipeline/SKILL.md](./skills/meeting-follow-up-pipeline/SKILL.md) | Turns a finished meeting into a debrief, decisions, action items, and proposed writebacks. |
| Exec Weekly Agenda Generator | [exec-weekly-agenda-generator/SKILL.md](./skills/exec-weekly-agenda-generator/SKILL.md) | Sweeps the week's meetings, chat, email, and calendar into a forced-ranked leadership agenda. |

This repo is also a Claude Code plugin (see [`.claude-plugin/plugin.json`](./.claude-plugin/plugin.json)), an OpenAI Codex plugin (see [`.codex-plugin/plugin.json`](./.codex-plugin/plugin.json)), and a GitHub Copilot CLI plugin (see [`.github/plugin/plugin.json`](./.github/plugin/plugin.json)) — its skills are discovered automatically from [`skills/`](./skills/) once installed on any of them.

## Installing a skill

- **Claude Code**: install as a plugin — `claude plugin marketplace add zapier/marketplace` then `claude plugin install wade-skills@zapier`.
- **OpenAI Codex**: `codex plugin marketplace add zapier/marketplace` then `codex plugin add wade-skills@zapier`.
- **GitHub Copilot CLI**: `copilot plugin marketplace add zapier/marketplace` then `copilot plugin install wade-skills@zapier`.
- **Cursor, or Claude Code without the plugin**: copy the skill's folder into `.cursor/skills/` or `.claude/skills/`. The `name` and `description` in its frontmatter is what triggers automatic invocation.
- **Claude Projects / a custom GPT / any chatbot**: paste the `SKILL.md` contents into the system prompt or project knowledge, then trigger it with the phrases listed under that skill's "When to Use" section.

Each skill has `[BRACKETED]` placeholders under a "Setup" section. Fill those in once for the user's stack (meeting-notes tool, CRM, leadership roster, etc.) before running it for real.

## Before you act

Read [NOTICE](./NOTICE) — it covers trademark use, the "not an official product" disclaimer, AI-output caveats, and the user's responsibility for data privacy when a skill touches meeting transcripts, email, or CRM records. These skills are built to propose actions and drafts, not auto-execute — keep a human in the loop when running them.

## License

MIT — see [LICENSE](./LICENSE).


---

## Espejo AI OS

This fork also contains the Espejo AI OS operating layer. These additions do not replace or modify the original Wade/Zapier skill files.

| Skill | File | What it does |
|---|---|---|
| Espejo War Room | [espejo-war-room/SKILL.md](./skills/espejo-war-room/SKILL.md) | Strategic decision council for prioritization, risk, revenue, customer value, and execution decisions. |
| Espejo Research / Intelligence | [espejo-research-intelligence/SKILL.md](./skills/espejo-research-intelligence/SKILL.md) | Research, verification, market and competitor intelligence, GitHub/open-source scouting, cost/dependency auditing, trend watch, and knowledge ingestion. |
| Espejo Growth Command | [espejo-growth-command/SKILL.md](./skills/espejo-growth-command/SKILL.md) | Customer acquisition, distribution, campaigns, experiments, and measurable growth execution. |
| Espejo Agentic Engineering | [espejo-agentic-engineering/SKILL.md](./skills/espejo-agentic-engineering/SKILL.md) | Builds and improves agents, software workflows, agent graphs, loops, tools, memory, evals, verification, security, cost control, and autonomous execution. |

### Espejo operating chain

Commander
→ Research / Intelligence
→ War Room
→ Growth Command
→ Agentic Engineering
→ Specialist Agents / Tools
→ Verification
→ Metrics
→ Learning
→ Next Decision

### Routing

- Research / Intelligence feeds War Room for strategic decisions.
- Research / Intelligence feeds Growth Command for customer acquisition and market signals.
- Research / Intelligence feeds Agentic Engineering for tools, repositories, integrations, and automation opportunities.
- War Room decides what should be done.
- Growth Command determines how to acquire attention, leads, customers, sales, retention, and referrals.
- Agentic Engineering designs and implements reliable agent/software execution systems.

### Universal operating rules

- Separate facts, assumptions, hypotheses, recommendations, and evidence.
- Verify before claiming completion.
- Use bounded loops with explicit stop conditions.
- Prefer the cheapest reliable model/tool for each job.
- Keep consequential spending, mass outreach, contracts, destructive changes, sensitive access, unapproved public publishing, and live pricing changes behind human approval.
- Record meaningful failures and convert them into prevention tests.
- Prefer reusable capabilities over repeated one-off implementations.
- Use current research when freshness matters.
