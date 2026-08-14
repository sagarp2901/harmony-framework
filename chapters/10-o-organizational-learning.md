# Chapter 10: O — Organizational Learning

*"AI adoption is a continuous learning journey."*

## The Playbook That Was Already Out of Date

Six months after the checkout postmortem, Jina's team had a genuinely good playbook: clear guidelines on AI-assisted development, a review process that caught most drift before it shipped, and a much better sense of where the real risks lived. She felt, for the first time since the rollout, like the organization had caught up.

Then the AI tooling itself changed. A major update to the coding assistant her teams used shifted its default behavior in ways nobody had asked for and few people noticed right away — it became more willing to make sweeping, multi-file changes on a single prompt, where the previous version had stuck to narrower edits. The playbook, written for the old behavior, didn't account for it. It took a near-miss — a well-intentioned engineer approving a much larger diff than they realized they'd asked for — to reveal that the guidelines needed updating again, less than two quarters after they'd been written.

## The Principle

AI tooling in this industry is not going to sit still long enough for any playbook to become permanent. A framework, a set of guidelines, a review process — all of it has a shelf life now, and the shelf life is shorter than most engineering leaders are used to planning for. Organizations that treat their AI practices as a one-time setup will find themselves, like Jina's team, quietly out of date within a couple of quarters, usually finding out the hard way rather than the easy one.

What worked instead was treating learning itself as a standing practice, not a project with an end date. That meant building habits for noticing when the tools had changed, sharing what different teams were learning in near real time, and revisiting guidelines on a cadence rather than only after something went wrong.

## What This Looks Like in Practice

- **A regular, low-effort forum for sharing what's actually being learned** — not a formal training program, but something closer to a standing channel or short recurring session where engineers surface what's changed, what surprised them, and what's stopped working.
- **A named owner for keeping AI-usage guidelines current**, with an explicit expectation that they'll be revisited on a cadence, not just when a near-miss forces the issue.
- **Room for experimentation with a clear enough boundary that it doesn't become the next ungoverned risk** — a way for engineers to try new capabilities and report back, without that experimentation happening invisibly in production.

## The Common Failure Mode

A playbook written once, trusted indefinitely, quietly falling out of sync with tools that keep changing underneath it. The gap is invisible until something exposes it, and by then it's usually already cost something.

## Questions Worth Asking Your Team

1. When your AI tooling last changed its behavior in a meaningful way, how long did it take your team to notice?
2. Do you have a standing, low-friction way for engineers to share what they're learning about these tools, or does that knowledge stay siloed with whoever happened to discover it?
3. Who owns keeping your AI-usage guidelines current, and when did they last actually update them?
4. If a new capability showed up in your AI tooling tomorrow, would your team find out about it through a deliberate process, or by accident?

---
