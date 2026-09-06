# Five-Advisors — Agent Instructions

This repo ships one skill, `five-advisors`, that stress-tests ideas with five
independent advisors (Devil's Advocate, First-Principles Questioner,
Opportunity Finder, Layman, Ruthless Executor), a cross-examination round, and
a chairman's verdict with an action list.

Trigger phrases: review my idea, evaluate this plan, is this viable, brainstorm
review, 审查我的想法, 这个方案可行吗, 帮我评估, 参谋, 多角度分析.

## How to make it work in YOUR tool

**Tools with an Agent Skills loader** (Codex, Claude Code, Hermes, Gemini CLI,
OpenCode, Cursor, Mistral Vibe, and 30+ others): install the skill. The
canonical copy is `five-advisors/SKILL.md`, a standard agentskills.io skill.
See the README table for each tool's skills directory, then copy or symlink
`five-advisors/` into it.

**Tools without a Skills loader** (AGENTS.md-only tools): when the user asks to
review an idea, READ the file `five-advisors/SKILL.md` and follow its workflow
verbatim — Round 1: five advisors speak independently; Round 2: they
cross-examine each other; Round 3: chairperson synthesizes verdict and action
list. Do not summarize or abridge the skill's rules.