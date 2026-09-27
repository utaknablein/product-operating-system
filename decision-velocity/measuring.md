# Measuring Decision Velocity

> Decision Velocity is a framework I developed for leadership teams. This page is the practical part: how to turn a [decision log](decision-log.md) into numbers a leadership team or a board can track.

## The idea in one paragraph

Organizations do not lack information. They lack the ability to turn it into decisions quickly and make those decisions stick. Most measure output (features shipped, hours saved) and never measure the step in between. Decision Velocity measures that step. It is also the right way to measure AI: not by hours saved, but by whether decisions got faster and better.

## Four numbers

### 1. Decision latency, by type

The median number of days from *raised* to *decided*, reported separately for each decision type.

> Report by type, never as one blended number. A pricing decision and a hiring decision have different natural speeds. A single average hides where the problem is.

### 2. Rework rate

The share of logged decisions that were remade within 90 days without new information.

> This is the number that surprises leadership teams most. A fast decision that gets remade twice is not fast.

### 3. Decision concentration

The share of logged decisions made by the top two decision owners.

> High concentration means the org routes too much to the top, and latency will rise as the business grows.

### 4. Agent effect

Latency and rework rate for agent-assisted decisions, compared with decisions people prepared alone. (Use the "Prepared by" column in the [decision log](decision-log.md).)

> This is how to measure AI in a product organization. Not hours saved, not agents deployed, but whether the decisions agents help prepare are made sooner and hold up better. If there is no difference after two quarters, the agents are busy, not useful.

## A simple scorecard

| | This quarter | Last quarter | Direction |
|---|---|---|---|
| Median latency: Roadmap | | | |
| Median latency: Launch | | | |
| Median latency: Build vs. buy | | | |
| Rework rate | | | |
| Decision concentration | | | |
| Agent effect: latency, assisted vs. not | | | |
| Agent effect: rework, assisted vs. not | | | |

Keep it to one page. Report it next to the business metrics, not in an appendix.

## What moves the numbers

In my experience, four changes do most of the work:

1. **One named owner per decision, and a date.** This alone cuts latency sharply, because most slow decisions are really unowned decisions.
2. **Write down "what would change our mind."** This cuts rework, because people who disagreed know what to watch instead of reopening the question.
3. **Push two-way doors down.** Decisions that are easy to reverse should be made by the person closest to the work, without escalation.
4. **Let agents prepare, never decide.** Agents are good at the slow part of a decision: gathering the thread, laying out options, checking what was decided before. The decision stays with a named person.

## Cautions

- **Do not optimize latency alone.** Speed on one-way doors can be reckless. Track rework next to latency so fast-and-wrong shows up.
- **Do not log everything.** A log that captures every small choice becomes a chore, then gets abandoned. Log the decisions that matter (see the [decision log](decision-log.md) criteria).
- **Do not use it to rank people.** The moment the log becomes a performance tool, people stop logging honestly.
