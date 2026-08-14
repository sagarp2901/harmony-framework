# Chapter 7: A — Architecture Stewardship

*"AI can accelerate construction, but humans must remain responsible for the blueprint."*

## Three Ways to Solve the Same Problem

Nobody decided to build three different caching layers for the same inventory-hold logic. That was the part of the checkout postmortem that stuck with Jina longest. Each of the three services had been built by a capable team, at a reasonable pace, solving the specific problem in front of them competently. The bug wasn't in any one implementation — each one worked, on its own terms. The bug was in the space between them, where three subtly different definitions of "how long should a hold last" quietly disagreed with each other under load.

Before AI tools, this kind of drift was rarer, for an unglamorous reason: building something new was expensive enough that engineers usually went looking for an existing solution first, simply because writing one from scratch cost more time than they had. That friction acted as an accidental discipline. AI removes the friction without replacing the discipline behind it. Writing a new implementation is now often faster than finding, reading, and understanding an existing one — which means the natural pressure that used to push engineers toward reuse and consistency has quietly gone away, and nothing has stepped in to replace it.

## The Principle

Architecture was never really about the code itself. It's about the decisions that outlive any single pull request: where system boundaries sit, what a service is and isn't responsible for, which tradeoffs the organization has already made on purpose and shouldn't have to re-litigate every sprint. AI can produce a correct-looking implementation of almost anything in minutes. It has no concept of the twelve other implementations already living in your codebase, and no stake in whether a thirteenth one is a good idea.

That means someone still has to hold the system in view on purpose — not as a side effect of code review, but as an explicit responsibility. Speed without a steward doesn't stay fast for long; it just moves the cost from "time to build" to "time spent untangling what got built," usually at a worse moment, under worse pressure, the way Team A discovered during a flash sale.

## What This Looks Like in Practice

- **Lightweight architecture review that scales with AI-assisted velocity.** If implementation now takes hours instead of days, review of the *approach* — not just the diff — needs to happen earlier and faster too, or it becomes the bottleneck nobody accounted for.
- **A living map of existing patterns**, kept current enough that "does something like this already exist" is a question an engineer can actually answer before generating a new implementation, not after.
- **Technical debt visibility that includes AI-introduced drift specifically** — not just the debt teams knowingly take on, but the kind that accumulates invisibly when nobody's watching for it.

## The Common Failure Mode

Three good decisions that don't know about each other. No single engineer, reviewer, or team did anything wrong in isolation — which is exactly what makes this failure mode hard to catch with normal code review. It only shows up when someone is explicitly responsible for looking across teams, not just within one pull request at a time.

## Questions Worth Asking Your Team

1. If two teams built AI-assisted solutions to a similar problem this quarter, would either of them know the other one existed?
2. Who, specifically, is responsible for noticing architectural drift across teams — and do they have time actually budgeted for it?
3. How would an engineer on your team currently find out whether something they're about to build already exists elsewhere in the codebase?
4. Has your technical debt tracking been updated to account for patterns introduced by AI-assisted development, or does it still only capture debt teams took on knowingly?

---
