# Five-Advisors Brain Trust

An OpenCode skill that stress-tests your ideas with five independent advisors.
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

Requires OpenCode. Clone this repo into your skills directory (e.g.
`~/.config/opencode/skills/`), or copy the folders individually:

```
opencode/skills/five-advisors/SKILL.md
opencode/command/five-advisors.md
```

Restart OpenCode after installing.

## Usage

- Prompt: "review my idea: ..." or any of 审查我的想法 / 这个方案可行吗 / 帮我评估
- Command: `/five-advisors <your idea>`

The command loads the skill and routes your input straight into the workflow.