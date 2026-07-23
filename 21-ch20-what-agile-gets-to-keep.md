# Chapter 20: What Agile Gets to Keep

This book has spent considerable time on what is wrong with modern Agile practice. It is worth being equally clear about what is right with it, because EASY is not a repudiation of Agile. It is a distillation. The goal is not to discard everything the last twenty-five years of software practice produced but to identify what in that body of practice was actually working and preserve it in a form that survives the AI transition.

Some of it does survive. The parts that survive are the parts that were never really about coordinating human labor at human speed. They were about learning fast, shipping often, and staying close to what users actually need. Those principles are as valid in an AI-augmented environment as they were in 2001. In some ways they are more valid, because AI makes it possible to act on them faster than anyone could have anticipated when the Agile Manifesto was written.

*What Was Always Right*

The Agile Manifesto's four core values hold up without qualification:[^1]

- Working software over comprehensive documentation
- Responding to change over following a plan
- Customer collaboration over contract negotiation
- Individuals and interactions over processes and tools

EASY does not contradict any of these. It enforces them more strictly than most Agile implementations do. A system with no documentation requirements, no planning ceremonies, and no process overhead beyond a two-column board is a more faithful expression of these values than a Jira implementation with seventeen custom fields and a quarterly roadmap review.

The practices that failed were not the values, which were always to the point. The machinery built on top of the values by an industry that needed to productize and sell a philosophy is what failed. EASY is about stripping away the machinery and returning to the values, which are still valid and useful.

*The Practices Worth Keeping*

Beyond the manifesto's values, several Agile-adjacent practices remain genuinely useful in an EASY environment:

- **Continuous delivery**: the practice of keeping software in a deployable state at all times and releasing frequently rather than in large batches. This is not a ceremony. It is an engineering discipline, and it is as important under EASY as under any other methodology. EASY actually reinforces continuous delivery by removing the sprint boundary that often becomes a de facto release gate.[^2]
- **Small batches**: the principle that smaller units of work move faster, generate earlier feedback, and carry less risk than large ones. EASY card sizing, discussed in Chapter 9, is a direct application of this principle. Smaller cards move to Done faster, and faster movement to Done means faster learning about whether the thing that was built is the right thing.
- **Customer feedback loops**: the practice of putting working software in front of real users regularly and adjusting based on what you learn. No project management methodology automates this, and EASY does not either. What EASY does is remove the process overhead that delays the shipping that makes feedback possible.
- **Cross-functional teams**: the organizational structure in which design, engineering, and product capabilities exist within the same team rather than being siloed into separate departments with formal handoff processes. EASY works best on cross-functional teams and poorly on teams that depend on ticket-based handoffs between functions.

*The Distinction That Matters*

The common thread in what Agile gets to keep is that none of it is about measuring human effort or coordinating human availability. Continuous delivery is about engineering practice. Small batches are about risk management. Customer feedback is about learning. Cross-functional teams are about organizational design. None of these practices break when AI joins the team, because none of them assumed the team was all-human in the first place.

**What broke under AI pressure was everything in Agile practice that was designed to answer the question "who is doing what, and how long will it take."** Story points, velocity, capacity planning, assignees, sprint planning, the daily standup: all of it was built to manage human labor. Remove the assumption of all-human labor and the practices built on it become unnecessary.

What remains is a philosophy about how to build software well: **ship often, learn fast, stay close to users, trust the people doing the work**. EASY is what that philosophy looks like when you stop building machinery on top of it.

---

[^1]: Beck, Kent, et al. *Manifesto for Agile Software Development*. 2001. Available at agilemanifesto.org.

[^2]: Humble, Jez, and David Farley. *Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation*. Boston: Addison-Wesley, 2010. The relationship between deployment frequency and organizational performance is further documented in the annual State of DevOps Reports produced by DORA (DevOps Research and Assessment), which consistently find that high-performing engineering organizations deploy significantly more frequently than low performers.
