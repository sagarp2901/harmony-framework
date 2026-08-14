# Chapter 14: Applying HARMONY-Y — A Worked Example

Everything in this chapter is fictional. The organization, its teams, and its numbers are a composite built to illustrate how the assessment works in practice, not a description of any real company.

## Meet Fictional Org: Northlight Systems

Northlight Systems is a mid-sized logistics software company, roughly 140 engineers across twelve teams, that adopted AI coding assistants organization-wide about eight months before this assessment. Leadership commissioned an internal review after noticing a pattern that should sound familiar by now: output metrics were strong, but a growing number of engineers, especially senior ones, had started raising informal concerns in retrospectives about code they didn't fully recognize and reviews that felt increasingly like guesswork.

## Step One: Honest Maturity Assessment

Northlight's leadership team worked through the Chapter 13 indicators, team by team, rather than as a single organization-wide guess. The results were uneven, which turned out to be the most useful finding of the whole exercise:

- Their **platform team**, responsible for the shared services other teams depended on, was operating close to **Level 3** — they had real governance, active architecture review, and a habit of tracking defect trends specifically for AI-assisted changes.
- Their **product teams**, working on customer-facing features under regular deadline pressure, were closer to **Level 1** — individual engineers had developed their own habits, with no shared standard and no coordinated review process for AI-assisted work.

This gap was the actual finding. Northlight wasn't uniformly behind. It had one part of the organization quietly protecting itself and another part quietly accumulating risk, and until this assessment, leadership had no way to see the difference.

## Step Two: Applying the Pillars Where the Gaps Were

Rather than launching an organization-wide initiative, Northlight's leadership focused first on closing the gap for the product teams, using the platform team's existing practices as a starting template rather than inventing something new.

- **H (Collaboration):** They wrote down, specifically, which categories of decisions on product teams required human design before AI-assisted implementation — largely borrowing the boundary the platform team had already been using informally.
- **A (Architecture):** They introduced a lightweight, fast architecture check for product teams — not a heavyweight review board, but a same-day conversation for any change that introduced a new pattern rather than reusing an existing one.
- **R (Governance):** They extended the platform team's data-handling guidance to product teams directly, rather than writing a separate policy from scratch, and made it easy to find inside the same tool engineers were already using daily.
- **M (Metrics):** Product team leadership reviews began pairing every velocity update with a defect-trend and rollback-rate figure, the same pairing the platform team had quietly been doing for months.
- **N (Risk):** Code review guidance was updated specifically to flag the kinds of subtle issues AI-generated code tends to produce, based on patterns the platform team had already documented from their own near-misses.

## Step Three: What Changed

Four months later, product team output had not measurably slowed — a detail leadership specifically called out, since the goal was never to reduce AI use. What changed was the shape of the outcomes: rollback rates on product team changes dropped by roughly a third, review conversations shifted noticeably from "does this pass tests" toward "why did we build it this way," and for the first time, leadership could point to a shared, current picture of AI-usage risk across the whole organization rather than just the platform team's corner of it.

Northlight didn't achieve Level 5. They moved from an uneven mix of Level 1 and Level 3 toward a more consistent Level 3 across the organization, with a few Level 4 habits — like the metrics pairing — starting to take hold. That's a realistic pace of change, and it's the pace most organizations applying this framework honestly should expect.

## The Takeaway

The most useful step in this process wasn't any single pillar. It was the assessment itself — the willingness to look honestly at where different parts of the organization actually stood, rather than assuming a single, organization-wide story was true everywhere. HARMONY-Y works best not as a program rolled out uniformly, but as a lens applied specifically to where the evidence says the gaps actually are.

---
