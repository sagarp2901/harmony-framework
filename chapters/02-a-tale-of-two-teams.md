# Chapter 2: A Tale of Two Teams

Jina's org had eleven teams by the time she started looking closely. Most sat somewhere in the middle — a bit more output, a bit more caution, nothing dramatic either way. But two teams stood far enough apart that they became her reference points for everything that followed. She didn't choose them for the story. They chose themselves, by how differently the same three months had gone for each of them.

**Team A** built customer-facing checkout services. When AI coding assistants rolled out, they leaned in immediately and completely. Within weeks, engineers were generating entire service scaffolds, tests, and documentation in a fraction of the time it used to take. Feature requests that once sat in a backlog for a sprint were live in staging within days. For the first month, it looked like the clearest AI success story in the company. Leadership used their velocity numbers in a slide deck.

By month two, the pattern Jina would later spend a year studying had already started. Nobody had sat down and designed how the new inventory-hold logic should work — it had simply emerged from a series of AI-assisted implementations, each one solving its immediate problem well and the larger problem not at all. Three separate services ended up computing similar values slightly differently, and nobody noticed until a customer was double-charged during a flash sale. The postmortem took longer than the original feature had taken to build. Senior engineers, the people best equipped to prevent exactly this kind of drift, found themselves spending most of their week reviewing and untangling AI-assisted changes instead of doing the design work only they could do.

**Team B** built the internal platform that other teams relied on for authentication and access control — a team with less room for error and, as it turned out, less appetite for moving fast without knowing why. They adopted the same AI tools on the same timeline. Their output went up too, just not as dramatically. What changed for them was less visible on a dashboard and more visible in how people spent their time. Engineers used AI to handle the repetitive parts — test scaffolding, documentation drafts, boilerplate — and put the time they got back into design conversations and threat modeling they'd never previously had time for. Their code review process didn't get faster. It got more thorough, because reviewers were now free to focus entirely on judgment instead of typing.

Six months in, Team B's incident rate had actually gone down from its pre-AI baseline. Their architecture, if anything, was cleaner than before — the extra design time had let them consolidate two overlapping internal libraries that had been on a wishlist for over a year.

If you'd only looked at pull request counts in month one, Team A won decisively. If you looked at what each team had actually become by month six, the comparison wasn't close — and it wasn't in Team A's favor.

## The Uncomfortable Part

The uncomfortable part of this story isn't that Team A did something wrong. Nobody on Team A cut a corner they knew was a corner. Every individual decision — ship this fast, trust this AI-generated implementation, move to the next ticket — was locally reasonable. That's what makes the pattern dangerous: it doesn't require anyone to make a bad call. It only requires an organization to let good local decisions accumulate without anyone responsible for the picture they add up to.

Team B wasn't smarter or more disciplined by nature. They worked in a domain — authentication — where the cost of a mistake was viscerally obvious to everyone on the team, so the habits that protected them were already partly in place before AI arrived. AI didn't build those habits. It amplified them, the same way it amplified Team A's absence of them.

That's the pattern this book keeps returning to, because it turned out to hold everywhere Jina looked afterward, not just on these two teams: **AI is a multiplier, not a corrective.** It doesn't push a team toward good practice or away from bad practice on its own. It takes whatever an organization already is, and gives it more of it, faster.

The rest of this book is about what "already being" a high-yield organization actually requires — deliberately, not by accident, and before the multiplier arrives rather than after.

---
