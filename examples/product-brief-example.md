# Product Brief: Unified Home Feed

> Worked example for [`templates/product-brief.md`](../templates/product-brief.md). Lumen is a fictional company; see [examples/README.md](README.md).

---

**Name:** Unified Home Feed
**Owner:** Priya Nair, Product lead, Home
**Decision this serves:** [Retire the legacy recommender](decision-memo-example.md), decided 11 March 2026. Once Recs v1 is gone, Home can be one ranked feed instead of two stacked rows.
**On roadmap:** ☒ Yes, item H-07 (replaces H-03 "Recs quality" and H-05 "Second-row refresh")

---

## The problem

Home is the first screen 1.2 million subscribers see, and today its top two rows are ranked by different systems. Returning subscribers scroll past the first row 61% of the time (March, all returning sessions), and in the last two rounds of user research, four of twelve participants described Home as "the same stuff twice." Support tagged 340 tickets in Q1 as "recommendations repetitive." The two-system layout is also why Home has not been redesigned in two years: nobody could agree which row to build around.

## The bet

We believe that replacing the two-row Home with a single v2-ranked feed, seeded by onboarding picks for new subscribers, for all subscribers will result in more sessions that start a listen from Home. We will know we are right when first-row listen starts rise and week-one engagement for new subscribers does not fall.

## How we will measure it

| | Metric | Today | Target | By when |
|---|---|---|---|---|
| Primary | Share of Home sessions with a listen started from the first row (returning subscribers) | 39% | 46% | 31 August 2026 |
| Guardrail | Week-one listens per new subscriber | 4.2 | No lower than 4.0 | Every weekly check from launch |

> The guardrail is the cold-start gap from the decision memo, made into a number the team checks weekly rather than a worry people repeat in meetings.

## Scope

**In:**
- One ranked feed on Home, v2 model, all platforms
- Onboarding picks used as the ranking seed for subscribers with fewer than three listens
- Removal of the second row and its "See all" page
- Dashboard: one "Home engagement" definition, published in the metrics catalog

**Out (on purpose):**
- Any new content type on Home (podcasts, live sessions). Those are H-09 and wait for this to land.
- Personalized push notifications from the feed. Different decision, different owner.
- A redesign of the player. Home only.
- Editorial "featured" slots. Editorial keeps its one pinned slot at the top, unchanged.

## What this replaces or stops

- Roadmap items H-03 (Recs quality, v1 tuning) and H-05 (Second-row refresh). Both close.
- The weekly "which row is right" review between Home and Discovery. Replaced by the single dashboard.

## Dependencies and risks

| Risk or dependency | Owner | What we will do about it |
|---|---|---|
| v2 cold-start quality for new subscribers | Tomás Herrera | Onboarding-seed approach ready by 15 June; guardrail checked weekly; new subscribers stay on v1 if the 15 June review fails (per the memo) |
| v1 switch-off date slips past 30 June | Dana Okafor | Feed ships on v2 regardless; v1 only continues for new subscribers if the guardrail is breached |
| Editorial objects to losing the second row | Priya Nair | Pinned slot stays; editorial consulted on 20 March, agreed |
| Metric definition dispute resurfaces | Mei Lin | One definition in the metrics catalog before launch; dashboards repointed |

## AI in this work

The feed is ranked by a model (v2), so AI decides the order of content on Home for every subscriber. It may decide ranking alone within the catalog of published content. It may not surface unpublished or age-restricted content, demote editorial's pinned slot, or change its own guardrail thresholds. Priya Nair is accountable for what the feed shows; Tomás Herrera for how the model behaves. When a subscriber reports a bad recommendation, it goes to a named reviewer, not back into the model unchecked.

---

**Agreed by:** Priya Nair (Product), Tomás Herrera (Engineering), Sam Whitfield (Design), Dana Okafor (business owner), 24 March 2026.
