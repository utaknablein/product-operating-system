# Product Operating System

The templates, rubrics and habits I use to run a product organization.

Most product orgs do not fail because they ship too little. They fail because they decide slowly, keep more roadmaps than anyone can count, and add work faster than they remove it. AI makes this worse, not better: building got cheap, so incoherence is now the expensive part.

This repo is how I keep a product org coherent and fast. It is opinionated, and it is short on purpose.

## What is here

| File | Use it when |
|---|---|
| [`principles.md`](principles.md) | You want to know why the rest of this repo looks the way it does |
| [`templates/decision-memo.md`](templates/decision-memo.md) | A decision needs more than a hallway conversation |
| [`templates/product-brief.md`](templates/product-brief.md) | Something is about to get built and you want one page everyone agrees on |
| [`templates/agent-role-card.md`](templates/agent-role-card.md) | An agent is joining the team and people need to know what it does and may decide |
| [`rubrics/prioritization.md`](rubrics/prioritization.md) | There is more on the list than the team can carry |
| [`rubrics/roadmap-coherence-check.md`](rubrics/roadmap-coherence-check.md) | The org feels busy but nothing seems to add up |
| [`decision-velocity/decision-log.md`](decision-velocity/decision-log.md) | You want to see where decisions actually get stuck |
| [`decision-velocity/measuring.md`](decision-velocity/measuring.md) | You want to turn that log into a number a board understands |

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
