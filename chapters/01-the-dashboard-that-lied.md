# Chapter 1: The Dashboard That Lied

Jina had been an engineering VP for six years, and she thought she knew what a good quarter looked like.

So when she opened the dashboard that Monday morning, she should have felt good. Pull requests were up 200%. Code volume had nearly tripled since the team rolled out AI coding assistants in Q1. Velocity charts pointed up and to the right, the way every leader wants them to. She forwarded the numbers to her CTO with a one-line note: *AI adoption is paying off.*

He replied within the hour, one word: *Great.*

For about three weeks, it was.

Then the on-call channel started getting louder. Not dramatically — nothing that would show up as a headline incident. Just a steady hum of small things: a null check that should have been there and wasn't, a config value that worked in staging and quietly didn't in production, a retry loop that someone had asked an AI assistant to "handle errors gracefully" and gotten exactly that, and nothing more specific. Individually, each one was a five-minute fix. Together, they were changing the shape of the week. Engineers who used to spend Friday afternoons wrapping up clean were now spending them triaging.

Code review time crept up too, which on the surface should have been a good sign — people were being careful. But when Jina sat in on a few reviews to see what was actually happening, she noticed something uncomfortable. The reviewers weren't reviewing a colleague's reasoning anymore. They were auditing a machine's guess, line by line, because they'd learned they couldn't fully trust it and couldn't fully ignore it either. That's a different, heavier kind of work than reviewing a peer's PR, and nobody had budgeted time for it.

Two of her architects asked to talk to her in the same week, separately, about the same thing. Not urgently — more like they were each hoping the other had already raised it. The gist, in both conversations, was the same: *we're moving fast, but I'm not sure I recognize the system we're building anymore.* Three services now solved variations of the same caching problem, each written by a different team, each generated with a different AI assistant, none of them aware the others existed. Nobody had decided this. It had simply accumulated, one fast, reasonable-looking pull request at a time.

Jina went back to her dashboard that Friday and looked at it differently. The number that had made her feel good on Monday — 200% more pull requests — hadn't moved. It was still true. But it had stopped telling her anything useful. It measured how much her teams had *done*. It said nothing about whether the organization was better off for having done it.

That gap — between what the dashboard showed and what was actually true — turned out to be the most important thing she noticed all quarter. Not because it was rare. Because it wasn't. She would later find the same gap, in different forms, at nearly every organization she talked to that had adopted AI tools seriously. Output had gone up. Whether that output was worth anything had quietly become a separate question — one nobody was tracking.

This book is about that gap, and what to do about it.

---
