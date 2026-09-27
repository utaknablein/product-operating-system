# Product Operating System

How I decide what gets funded, what gets cut, and how we know it worked.

Most product organizations do not fail because they ship too little. They fail because they decide slowly, run more roadmaps than anyone can count, and add work faster than they remove it. As CPO at iHeartMedia I inherited exactly that: several roadmaps, three analytics platforms and a long tail of features almost nobody used. We merged the roadmaps into one, consolidated the analytics into one, retired the low-use features, and moved roadmap decisions from campaign calendars to behavioral data. This repo is the system that came out of that work, rebuilt for a world where agents do much of the preparation.

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

## How to use it

Copy what is useful, cut what is not. These are starting points, not rules. If a section in a template never changes anyone's mind, delete it. That is the whole philosophy in one sentence.

## Related

- [`engine-diagnostic`](https://github.com/utaknablein/engine-diagnostic): an AI maturity diagnostic for leadership teams, built on my ENGINE framework
- [`agent-workflows`](https://github.com/utaknablein/agent-workflows): the agents that work with these templates, with triggers, permissions and a scorecard
- More about me on my [profile](https://github.com/utaknablein)
