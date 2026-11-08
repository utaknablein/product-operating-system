# Decision Memo: Retire the legacy recommender

> Worked example for [`templates/decision-memo.md`](../templates/decision-memo.md). Lumen is a fictional company; see [examples/README.md](README.md).

---

**Decision:** Do we retire the legacy recommendations service (Recs v1) and move all surfaces to the ranking model (Recs v2) before the Q3 planning cycle?

**Owner:** Dana Okafor, VP Product

**Decide by:** 14 March 2026

**Prepared by:** ☐ Person  ☒ Agent-assisted *(the decision memo agent drafted this from the #recs-migration thread after it passed 20 messages without a decision; Priya Nair, product lead for Home, checked it)*

**Type:** ☒ One-way door (hard to reverse)  ☐ Two-way door (easy to reverse)

> Once v1 is switched off, its training pipeline and the two engineers who understand it move on. Bringing it back after Q3 would cost roughly a quarter of work.

---

## Why now

Two recommenders means two definitions of "recommended" in every dashboard, two on-call rotations, and a Home screen where the top row and the second row are ranked by different systems. The engineers who maintain v1 have asked to move to v2 work by April; if we do not decide by mid-March, we lose them to the Search team and v1 becomes unowned. Infrastructure cost for running both is about $38k a month.

## Options

| | Option | What it gets us | What it costs | What it rules out |
|---|---|---|---|---|
| A | Retire v1 by end of Q2; v2 takes over all five surfaces | One system, one metric, $38k/month back, two engineers freed for v2 quality | Four weeks of migration work; a known gap in v2 for new subscribers with under three listens (cold start) | Running an A/B between the two systems after Q2 |
| B | Keep v1 for cold-start users only; v2 everywhere else | Protects week-one engagement for new subscribers | Keeps both pipelines alive indefinitely; the "two metrics" problem does not go away; v1 still needs an owner | Freeing the two engineers |
| C | *Do nothing*: keep both as they are | No migration risk this quarter | $38k/month, two on-call rotations, the dashboard dispute continues, v1 becomes unowned in April anyway | A clean Home redesign in Q3 |

> Option B sounds like a compromise. It is actually Option C with a better name: both systems stay, and the hardest part (cold start) is the part nobody owns.

## Recommendation

Option A. Retire v1 by 30 June, and give the freed engineers one explicit job: close the v2 cold-start gap by the same date, using the first-session onboarding picks as a seed. We accept a measured dip in week-one engagement for new subscribers during the migration, with a guardrail below.

## What would change our mind

1. If the cold-start gap in v2 cannot be closed to within 5% of v1 on week-one listens by 15 June, we pause the switch-off for new subscribers only and revisit on 1 July.
2. If the v1 engineers can be retained on v1 past April (they currently cannot), the urgency drops and Option B becomes worth a proper test.

## What this stops

- The v1 training pipeline, its on-call rotation and its dashboard.
- The "Recs quality" roadmap line owned by the Discovery team, which was a v1 tuning effort. The team moves to v2 cold start.
- The planned Q3 A/B of v1 versus v2. The decision replaces the test.

## Who was consulted

- **Priya Nair, Product lead, Home:** for A. "We have been arguing about which row is right for a year."
- **Tomás Herrera, Engineering lead, Discovery:** for A, with the cold-start guardrail. Would have preferred B six months ago; says the window has passed.
- **Mei Lin, Data science:** against A as written. Believes the cold-start gap is larger than reported (v2 has been measured on returning users only). Asked that the 5% guardrail be measured on new subscribers specifically. Agreed to commit if that is written down. It is, above.
- **Finance (Jon Adeyemi):** for A. Wants the $38k/month shown against the migration cost in the Q2 review.

---

## Decision record

- **Decided:** Option A, 11 March 2026
- **Decided by:** Dana Okafor
- **Days from memo to decision:** 6 (raised 5 March, logged as entry #4 in the [decision log](decision-log-example.md))
- **Review on:** 15 June 2026, against "what would change our mind" item 1
