# Chapter 9: M — Metrics Redefinition

*"The best engineering organizations will not be those producing the most code. They will be those producing the most value."*

## The Number That Stopped Meaning Anything

Jina kept coming back to the number from that first Monday: 200%. Pull requests up 200%, and for three weeks, that number had made her feel like the organization was winning. It hadn't been wrong, exactly. It had just stopped being connected to the thing she actually cared about.

Lines of code, commit counts, and story points had always been imperfect proxies for value — every engineering leader knew that, in theory, even while using them daily in practice. What made them tolerable for so long was that the imperfection was bounded. A human being can only write so much code in a day, so even a flawed proxy stayed roughly in the neighborhood of real effort. AI removes that bound. Output can now scale by an order of magnitude without the underlying judgment, care, or effort scaling anywhere close to the same degree. The old proxies didn't get slightly less accurate. They became actively misleading, precisely when leaders were leaning on them hardest to justify the return on AI investment.

## The Principle

The organizations that come out ahead in the next several years will not be the ones who can point to the most code generated, the most tickets closed, or the fastest velocity chart. They'll be the ones who quietly shifted what they measure — toward outcomes that are harder to game and closer to what actually matters — before the old numbers led them somewhere they didn't want to go.

This doesn't mean abandoning activity metrics entirely. Deployment frequency and lead time are still useful signals, just no longer sufficient ones on their own. What has to sit alongside them is a set of measurements that ask a different question: not "how much did we do," but "how much of what we did is still standing, still trusted, and still worth having."

## What This Looks Like in Practice

- **Defect and incident trends tracked specifically for AI-assisted work**, separated out where possible from human-authored changes, so drift becomes visible before it becomes a postmortem.
- **Review time treated as a signal, not just a cost.** A rising review-to-merge ratio isn't automatically a problem — it can mean reviewers are doing real diligence on AI-assisted changes. What matters is whether the organization is watching that trend on purpose, rather than optimizing it away.
- **Customer and reliability outcomes given at least equal weight to velocity in any AI adoption report.** If a slide about AI's impact only ever shows output metrics, that's itself a signal worth noticing.

## The Common Failure Mode

Celebrating a velocity chart without checking what's underneath it — the exact mistake the CTO's one-word reply, *Great*, nearly locked in before the cracks showed. Not because anyone was careless, but because the old metrics were the only ones anyone had learned to look at first.

## Questions Worth Asking Your Team

1. If your team's AI adoption were judged purely on the metrics in your current dashboard, would that judgment hold up six months from now?
2. Are you tracking defect and incident rates in a way that would let you notice if AI-assisted code specifically started causing more problems than human-authored code?
3. When was the last time a leadership update on AI adoption led with a reliability or customer-impact metric instead of an output metric?
4. What would have to be true for your organization to feel confident saying "we produced less, and it was a better quarter"?

---
