# Chapter 4: Four Questions Nobody Had Good Answers To

Once Jina started looking for the gap between output and value, she couldn't stop finding it. It showed up in postmortems, in planning meetings, in the offhand comments engineers made when they thought nobody was listening closely. Underneath most of it, she found the same four questions surfacing again and again — questions her organization had never needed to answer before, because the old assumptions had made them unnecessary.

## Who Owns a Decision the AI Made?

The checkout postmortem that closed out Team A's second month raised this question directly, and nobody in the room had a clean answer. The AI assistant had suggested the rounding logic that caused the double-charge. An engineer had accepted the suggestion without deeply questioning it, because it looked correct and passed the tests that existed at the time. A reviewer had approved the pull request, because the diff was small and the tests were green.

So who was accountable? Not the AI — accountability has to attach to someone who can learn from the mistake and change their behavior, and a language model does neither. Not quite the engineer alone, either, in the way blame usually attaches to a human author, because the reasoning behind the choice was never fully theirs to begin with. The honest answer, once Jina's team worked through it, was that ownership had to be a property of the *process*, not any single person in it. If nobody explicitly owns the decision to accept AI-generated logic into production, then in practice, no one does — and a null owner is precisely the condition under which small mistakes turn into repeated ones.

## What Does Productive Even Mean Now?

Marcus, from Team A, had by every traditional measure become the most productive engineer in the company that quarter. He also, without ever being reckless on purpose, became one of the largest sources of unreviewed architectural drift in the organization. Both things were true at once, and the dashboard only showed one of them.

This is the question every engineering leader eventually has to sit with once AI enters the picture: if a tool can make raw output cheap, what should "high performer" mean instead? Jina's org didn't arrive at a perfect answer, but they arrived at a useful one — productivity had to be redefined around the durability of what got built, not the speed of building it. Chapter 9 goes into this in depth.

## Who Is Protecting the Architecture?

Nobody on Team A was assigned to prevent architectural drift, because nobody had ever needed to be. Before AI, the sheer effort required to build something new acted as a natural brake — engineers reused existing patterns partly because building something new from scratch was expensive, and that expense happened to double as a discipline. AI removes the expense without replacing the discipline. Writing a new, slightly different implementation of something that already exists became, almost overnight, easier than finding and understanding the existing one.

That meant architectural stewardship, which used to be a byproduct of friction, had to become a deliberate role again. Someone had to hold the whole system in view on purpose, because the system was no longer going to hold its own shape by default.

## What New Risks Did We Just Invite In?

The double-charge incident was a business problem before it was anything else, but Jina's security team flagged a second, quieter risk in the same quarter: an engineer had pasted a chunk of production configuration, complete with a service credential, into a prompt to an AI assistant while asking for help debugging a connection issue. Nothing came of it — the assistant didn't retain or leak the credential — but it was close enough to a real exposure that it changed how the security team thought about the problem. AI tools create a new category of pathway for sensitive data to travel through, and most organizations, Jina's included, had written their data-handling policies before that pathway existed.

None of these four questions had good answers sitting on the shelf. Jina's organization had to build the answers, deliberately, the same way every organization now has to. What follows in this book is the shape those answers took — organized into seven pillars that, together, form HARMONY-Y.

---
