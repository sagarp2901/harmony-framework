# Chapter 11: N — Navigating AI Risk

*"The goal is not eliminating risk. The goal is managing risk intelligently."*

## What a Small Risk Looks Like Before It's a Big One

None of Team A's problems arrived as a single dramatic failure. That was the part Jina found hardest to explain to people who hadn't lived through it. The double-charge incident had roots in a rounding decision that, on its own, looked entirely reasonable in code review. The near-miss with the leaked credential was a single engineer, under time pressure, doing something thousands of engineers do every day without incident. The architectural drift across three services happened one locally sensible pull request at a time. Every individual risk, examined in isolation, looked survivable. What made them dangerous was that nobody was watching for the pattern they formed together.

## The Principle

AI introduces failure modes that traditional software practices weren't built to catch, precisely because those practices assume a human wrote the code with full context and reasonable care. Generated code can look syntactically clean and logically sound while quietly containing a subtle security gap. A confident, well-formatted recommendation can be wrong in a way that's hard to catch specifically because it doesn't look uncertain. Sensitive data can drift into a workflow it was never meant to touch, not through malice, but through the ordinary act of describing a problem clearly enough to get help with it.

None of this means treating AI as untrustworthy in a way that cancels out its value. It means building the habit of catching small risks while they're still small — before they've had a chance to compound into the kind of problem that shows up in a postmortem instead of a routine review.

## What This Looks Like in Practice

- **Validation that assumes AI-generated output deserves the same scrutiny as an unfamiliar contributor's first pull request** — not more suspicion than a trusted colleague's work, but not automatically less, either.
- **Security review specifically tuned to the kinds of mistakes AI tends to make** — subtle logic gaps, plausible-looking but insecure defaults — rather than only the categories of mistake a security review was originally designed to catch.
- **Operational safeguards that assume some failures will get through anyway**, because they will: fast rollback paths, clear ownership during incidents, and a bias toward catching problems in minutes rather than days.

## The Common Failure Mode

Waiting for a risk to become visible before treating it as real. By the time an issue is big enough to show up in an incident report, it has usually already been small and invisible for weeks.

## Questions Worth Asking Your Team

1. Does your code review process treat AI-generated code with a level of scrutiny closer to a new contributor's work, or closer to a trusted teammate's — and is that the right calibration?
2. Has your security review process been updated specifically for the kinds of mistakes AI tools tend to introduce, or does it still only cover the categories it was originally designed for?
3. If a small, AI-related risk emerged on your team this week, is there a clear, low-friction way for someone to flag it before it compounds?
4. How quickly could your team roll back an AI-assisted change if it turned out, after the fact, to be wrong in a way nobody caught in review?

---
