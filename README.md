# Product Operating System

How I decide what gets funded, what gets cut, and how we know it worked.

Most product organizations do not fail because they ship too little. They fail because they decide slowly, run more roadmaps than anyone can count, and add work faster than they remove it. As CPO at iHeartMedia I inherited exactly that: several roadmaps, three analytics platforms and a long tail of features almost nobody used. We merged the roadmaps into one, consolidated the analytics into one, retired the low-use features, and moved roadmap decisions from campaign calendars to behavioral data. This repo is the system that came out of that work, rebuilt for a world where agents do much of the preparation.

**Start here:** [write your first decision memo in 30 minutes](QUICKSTART.md), for a decision your team is actually stuck on. Every template is also filled in for one fictional company in [`examples/`](examples/), so you can see what a finished memo, brief, role card and log look like before you write your own.

## For the executive team

| File | Use it when |
|---|---|
| [`decision-velocity/measuring.md`](decision-velocity/measuring.md) | You want a number the board understands for how fast the company decides |
| [`rubrics/roadmap-coherence-check.md`](rubrics/roadmap-coherence-check.md) | The organization feels busy but the portfolio does not add up to the strategy |
| [`decision-velocity/decision-log.md`](decision-velocity/decision-log.md) | Settled decisions keep getting re-argued |
| [`principles.md`](principles.md) | You want the operating principles behind everything else here |

## For the teams

| File | Use it when |
|---|---|
| [`rubrics/prioritization.md`](rubrics/prioritization.md) | There is more on the list than the team can carry |
| [`templates/decision-memo.md`](templates/decision-memo.md) | A decision needs more than a hallway conversation |
| [`templates/product-brief.md`](templates/product-brief.md) | Something is about to get built and you want one page everyone agrees on |
| [`templates/agent-role-card.md`](templates/agent-role-card.md) | An agent is joining the team and people need to know what it does and may decide |

## How the pieces fit

```
principles ──> decide ──────────> build ─────────> learn
               decision memo      product brief     decision log
               prioritization                       decision velocity
               coherence check
```

Every template starts with the decision, not the feature. A brief without a named decision owner and a date is a wish list.

## Built for teams of people and agents

More and more of the preparation in a product org is done by agents: drafting memos, checking roadmaps, synthesizing research. This repo assumes that. Every agent gets a [role card](templates/agent-role-card.md) and a named owner, agents prepare but never decide, and the [decision log](decision-velocity/decision-log.md) records which decisions agents helped prepare, so you can measure whether they make the organization faster. The agents themselves are specified in [`agent-workflows`](https://github.com/utaknablein/agent-workflows).

## In practice

When I became CPO at iHeartMedia the product organisation was running thirteen roadmaps. Each was defensible on its own. Together they added up to more work than the company had engineers, and nobody could say what the whole was for. We merged them into one roadmap with explicit sequencing, and aligned every line on it to the same north star metrics and KPIs, to payback, and to its effect on margin. The roadmap deliberately mixed quick wins with foundation work that paid off later; a shared component library is slow to build and makes everything after it faster. We also consolidated the analytics stack, because three platforms produce three versions of the truth and a recurring meeting about which one is right. The templates in this repo are what that work left behind. The decision memo exists because the hardest part was never the roadmap. It was saying out loud what we would stop.

## Worked examples

| Example | Shows |
|---|---|
| [Decision memo](examples/decision-memo-example.md) | A one-page memo with a real "do nothing" row and a recorded disagreement |
| [Product brief](examples/product-brief-example.md) | One primary metric, one guardrail, and an "out" list that protects the team |
| [Agent role card](examples/agent-role-card-example.md) | Decision rights for an agent, "never" column first, with a quarter's review filled in |
| [Decision log](examples/decision-log-example.md) | Ten decisions from one quarter and what the four monthly readings say about them |

All four follow one decision at the same fictional company, so you can see how a memo becomes a brief becomes a log entry.

## How to use it

Copy what is useful, cut what is not. These are starting points, not rules. If a section in a template never changes anyone's mind, delete it. That is the whole philosophy in one sentence.

## Related

- [`engine-diagnostic`](https://github.com/utaknablein/engine-diagnostic): an AI maturity diagnostic for leadership teams, built on my ENGINE framework
- [`agent-workflows`](https://github.com/utaknablein/agent-workflows): the agents that work with these templates, with triggers, permissions and a scorecard
- More about me on my [profile](https://github.com/utaknablein)
