# Agent Role Card: Decision memo agent

> Worked example for [`templates/agent-role-card.md`](../templates/agent-role-card.md). This is the agent that drafted the [example decision memo](decision-memo-example.md). Its full technical spec is in [`agent-workflows`](https://github.com/utaknablein/agent-workflows/blob/main/workflows/decision-memo-agent.md). Lumen is a fictional company; see [examples/README.md](README.md).

---

**Agent:** Decision memo agent
**Role in one sentence:** When a discussion thread stalls, it drafts a one-page decision memo from the thread so a named person can decide instead of the thread continuing.
**Accountable owner:** Dana Okafor, VP Product
**Works with:** Product leads (receive the draft), the decision owner named in the thread, the decision log (where the outcome is recorded)
**Status:** ☐ Pilot  ☒ Live  ☐ Under review  ☐ Retired

---

## Responsibilities

| This agent... | For this decision or work |
|---|---|
| **Prepares** | A first-draft decision memo for any product thread that passes 20 messages or 7 days without a recorded decision |
| **Checks** | The decision log for an earlier decision on the same question, and flags it in the draft if one exists |
| **Never decides** | Which option is chosen, who the owner is, the decide-by date, or whether the memo is sent beyond the product team |

## Decision rights

| May do alone | Needs a person's approval | Must never do |
|---|---|---|
| Read product channels and the decision log | Post the draft to the thread (the product lead reviews first) | Choose or recommend an option as if it were the team's view |
| Draft the memo, including the options table and a "do nothing" row | Name a decision owner (it proposes; the product lead confirms) | Send anything outside the product organization |
| Propose a decide-by date from the thread's own deadlines | Mark the decision as made | Quote a person's message out of context, or attribute a position someone did not take |
| Write "what would change our mind" from disagreements in the thread | | Read channels marked confidential (legal, people, M&A) |

> The "never" column was written first. The last row exists because the first version of this agent summarized a compensation thread it should not have been able to see.

## Hand-offs

The draft goes to the product lead for the area as a private message, not to the thread. The product lead edits, confirms the owner and date, then posts it. Nothing reaches the decision owner until a person has read it. After the decision, the product lead logs it; the agent does not write to the log.

## How we review it

Quarterly, by Dana Okafor, like any team member:

- Is its work accepted without substantial rework? *Q1: 9 of 11 drafts posted with minor edits. Two were discarded: one thread was not a decision, one was already decided and not logged (which is itself a finding).*
- Does it catch things the team would have missed? *Twice it found an earlier decision on the same question in the log.*
- Has it made an error, or invented a source? *Once, in January, it attributed a position to the wrong person. Fixed by requiring quotes to carry the message link.*
- Does it escalate when it should? *Yes. It stops and asks when a thread names more than one owner.*
- **Are the decisions it supports faster or better?** *See the [decision log](decision-log-example.md): agent-assisted decisions, median 6 days; others, median 16.*

Verdict: ☒ Keep  ☐ Fix  ☐ Retire

## What the team should know

It only reads the thread. If the real discussion happened in a meeting, the memo will miss it; add a two-line meeting note to the thread before it fires. It cannot see Figma, docs or dashboards linked in the thread, so it will say "the thread references a dashboard" rather than quote the number. If a draft misrepresents your position, reply in the thread with a correction and tell Priya Nair; the draft is withdrawn and redone.
