# Decision Log: Lumen, Q1 2026

> Worked example for [`decision-velocity/decision-log.md`](../decision-velocity/decision-log.md). One quarter of a fictional company's log, then the four monthly readings. Lumen is a fictional company; see [examples/README.md](README.md).

## The log

| # | Decision | Type | Owner | Prepared by | Raised | Decided | Days | Door | Revisited? | Link |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Raise annual plan price from $89 to $99 for new subscribers | Pricing | J. Adeyemi | Person | 2026-01-06 | 2026-01-27 | 21 | Two-way | No | memo |
| 2 | Build in-house transcript search or license a vendor | Build vs. buy | T. Herrera | Agent-assisted | 2026-01-12 | 2026-01-19 | 7 | One-way | No | memo |
| 3 | Hire a second data scientist for Discovery | Hiring | D. Okafor | Person | 2026-01-15 | 2026-02-20 | 36 | Two-way | No | thread |
| 4 | Retire Recs v1 before Q3 | Stop/sunset | D. Okafor | Agent-assisted | 2026-03-05 | 2026-03-11 | 6 | One-way | No | [memo](decision-memo-example.md) |
| 5 | Launch Sleep Stories in the Android app before iOS | Launch | P. Nair | Person | 2026-02-02 | 2026-02-13 | 11 | Two-way | **Yes, 2026-03-18** | thread |
| 6 | Move the Q2 roadmap review from monthly to fortnightly | Policy | D. Okafor | Person | 2026-02-10 | 2026-02-10 | 0 | Two-way | No | note |
| 7 | Drop the "Daily Mix" feature (under 2% weekly use) | Stop/sunset | P. Nair | Agent-assisted | 2026-02-17 | 2026-02-24 | 7 | One-way | No | memo |
| 8 | Allow the support agent to issue refunds under $20 without review | Policy | S. Whitfield | Person | 2026-02-24 | 2026-03-20 | 24 | One-way | No | memo |
| 9 | Relaunch Sleep Stories on both platforms at once | Launch | P. Nair | Person | 2026-03-18 | 2026-03-25 | 7 | Two-way | *remake of #5* | thread |
| 10 | Replace three analytics tools with one | Build vs. buy | T. Herrera | Agent-assisted | 2026-03-09 | 2026-03-16 | 7 | One-way | No | memo |

## Reading it: the four monthly checks

**1. Median days by type**

| Type | Decisions | Median days |
|---|---|---|
| Hiring | 1 | 36 |
| Policy | 2 | 12 |
| Pricing | 1 | 21 |
| Launch | 2 | 9 |
| Build vs. buy | 2 | 7 |
| Stop/sunset | 2 | 6.5 |

Hiring is the outlier. Entry #3 took 36 days because the role was raised in a thread with no owner until 3 February; the actual decision, once Dana owned it, took eight days. The slow part was not the deciding. It was the four weeks before anyone was asked to decide. That is the most common shape of a slow decision.

**2. Revisited decisions**

One: Sleep Stories (#5, remade as #9). The February decision to launch Android first was made in a thread with no memo and no "what would change our mind." When iOS engineering freed up in March, the question was reopened from scratch instead of checked against a recorded condition. Cost: five weeks of a feature on one platform and a second round of the same argument. The fix is not faster deciding. It is writing down, in February, "we go Android first unless iOS capacity opens before April."

**3. Who decides**

Dana Okafor owns 3 of 10; Priya Nair owns 3. The top two owners hold 60% of the log. Two of Dana's three (#3 hiring, #6 policy) are two-way doors that could have been decided one level down. Decision concentration will rise as Lumen grows unless two-way doors are pushed to the product leads now.

**4. Agent-assisted versus not**

| Prepared by | Decisions | Median days | Revisited |
|---|---|---|---|
| Agent-assisted | 4 | 7 | 0 |
| Person | 6 | 16 | 1 |

Agent-assisted decisions were made faster and none were reopened. Two cautions before claiming victory. First, the agent only fires on threads that are already stalled, so it is selecting for decisions that were about to get attention anyway. Second, four is not a sample. After two quarters this comparison means something; after one it is a reason to keep logging.

## What Lumen's leadership team took from this quarter

Three things, each one a decision rather than an observation:

1. Two-way doors on hiring and internal policy move to the product leads. Dana reviews the log, not the decisions.
2. Every launch decision gets a memo, even a short one, because the only remade decision this quarter was the one without a memo.
3. The decision memo agent stays live and gets a second quarter before anyone reports its numbers to the board.

For turning these readings into a one-page scorecard, see [measuring.md](../decision-velocity/measuring.md).
