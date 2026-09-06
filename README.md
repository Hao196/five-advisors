# Five-Advisors Brain Trust

A standard Agent Skills (agentskills.io) skill that stress-tests your ideas
with five independent advisors. Works in Codex, Claude Code, Hermes, Gemini
CLI, OpenCode, and 30+ supporting agents.
Share a concept, plan, topic, decision, or business idea and get a structured
multi-angle review: independent opinions first, cross-examination after, and
a chairman's verdict with an action list at the end.

## The Five Advisors

- **Devil's Advocate** — attacks your idea with real data, failure cases, and
  counterexamples to find where it most likely fails.
- **First-Principles Questioner** — digs to the bottom, exposing assumptions
  you've never actually verified.
- **Opportunity Finder** — hunts for options beyond the two you already thought
  of (c, d, e instead of just a and b).
- **Layman** — knows nothing about your industry and asks the dumb-simple
  questions experts always skip.
- **Ruthless Executor** — only cares about the first step tomorrow morning.
  Anything that can't be acted on gets killed.

## Workflow

1. **Round 1 — Independent Review**: each advisor speaks alone, no groupthink.
2. **Round 2 — Cross-Examination**: advisors challenge each other's points.
3. **Round 3 — Chairman Synthesis**: consensus and disputes are settled, then a
   verdict (support / conditional / reject / test first), an action list
   (today / this week / quit decision), and the one critical unknown.

No fabricated data. No rubber-stamp "looks good". If all five agree, the
process failed.

## File Layout

```
five-advisors/SKILL.md      the skill definition
commands/five-advisors.md   the /five-advisors command entry point
```

## Install

One `SKILL.md`, every platform. Copy (or symlink) it into your agent's skills
directory, then restart the agent:

| Platform          | Location                                  |
|-------------------|-------------------------------------------|
| Codex             | `~/.agents/skills/` or `~/.codex/skills/` |
| Claude Code       | `~/.claude/skills/`                        |
| Hermes Agent      | `~/.hermes/skills/`                        |
| Gemini CLI        | `~/.gemini/skills/`                        |
| OpenCode          | `~/.config/opencode/skills/`               |
| Any project       | `.agents/skills/` in the repo          |

`commands/five-advisors.md` is an optional OpenCode `/command` shortcut that
loads the skill and routes your input into the workflow.

## Usage

- Prompt: "review my idea: ..." or any of 审查我的想法 / 这个方案可行吗 / 帮我评估
- Command: `/five-advisors <your idea>`

The command loads the skill and routes your input straight into the workflow.