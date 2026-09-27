# Prioritization Rubric

> Use this when there's more on the list than the team can carry. It isn't a formula that makes the decision for you. It's a way to make the trade-offs visible so the conversation is about the right things.

## Step 1: Pass the gates

Before anything gets scored, it has to answer yes to all three. If it can't, it doesn't go on the list yet.

1. **Does it serve the strategy we already agreed?** Name the goal. "It's a good idea" is not a goal.
2. **Does it have one owner?** A name, not a team.
3. **Does it say what it replaces or stops?** See [Subtract before you add](../principles.md#4-subtract-before-you-add).

## Step 2: Score what passed

Score each item 1 (low) to 3 (high). Keep it coarse. Arguing about a 7 versus an 8 is a sign the scale is too fine to be honest.

| Criterion | Question | Weight |
|---|---|---|
| **Impact** | If it works, how much does the primary metric move? | ×3 |
| **Confidence** | How good is our evidence that it will work? | ×2 |
| **Decision leverage** | Does it make future decisions faster or better (data, tooling, clarity)? | ×2 |
| **Coherence** | Does it strengthen what we already have, or add a new thing to maintain? | ×1 |
| **Effort** | How much of the team does it take? *(scored in reverse: 3 = small)* | ×2 |

**Score = sum of (score × weight).** Maximum 30.

> Why "decision leverage" gets its own line: this is where platform and plumbing work finally gets credit. A search index or a clean data model rarely wins on impact alone, but it makes every later decision cheaper.

## Step 3: Sanity-check the top of the list

Before you publish the ranked list, ask:

- **Is the plumbing share protected?** I reserve a fixed share of capacity for platform work so it doesn't have to win this vote every quarter.
- **Is anything here only because someone senior asked?** That can be fine, but say so out loud.
- **What did we stop?** If the new list is longer than the old one and nothing was removed, go back to Step 1.

## Step 4: Write down the call

The ranked list is an output of a decision. Record it like one, with a [decision memo](../templates/decision-memo.md) if it's contested, and log it in the [decision log](../decision-velocity/decision-log.md).
