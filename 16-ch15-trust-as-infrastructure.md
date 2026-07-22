# Part Three: The Cultural Shift

---

# Chapter 15: Trust as Infrastructure

Part Two described a system with no assignees, no due dates, no status tracking, and no mandatory ceremonies. What it did not say explicitly is what that system requires in order to function. EASY is not self-enforcing. No methodology is. The practices are simple, but the conditions that make them possible are not trivial, and the most important of those conditions is trust.

Not trust in an abstract, inspirational sense. Trust in a specific, operational sense: confidence that the people on your team will pull work without being assigned to it, complete it without being chased, declare it done only when it actually is done, and say something when they are stuck rather than letting a card sit quietly in the Not Done column. These are not heroic behaviors. They are baseline professional behaviors. But they are behaviors that many organizational systems actively undermine by replacing them with compliance mechanisms, and when the compliance mechanisms are removed, the behaviors have to be there or the system fails.

*What Trust Actually Means*

In the EASY context, trust has three components:

- **Autonomy trust**: confidence that team members will identify the most important work and pursue it without needing to be directed task by task
- **Honesty trust**: confidence that a card moved to Done reflects work that is genuinely complete, not work that is complete enough to stop talking about
- **Communication trust**: confidence that blockers, questions, and concerns will surface through conversation rather than through ticket metadata or status fields

These three components are interdependent. A team with strong autonomy trust but weak honesty trust will move cards to Done prematurely and ship unreliable software. A team with strong honesty trust but weak communication trust will leave cards stuck in Not Done without escalating the reasons, and the board will accurately reflect a team that is not making progress without anyone knowing why.

**EASY does not create these behaviors. It assumes them.** This is a feature of the system, not a gap. A methodology that tries to enforce trustworthy behavior through process controls is a methodology that has already lost the argument. If you need your ticketing system to catch developers who are not being honest about the state of their work, your problem is not your ticketing system.

*Trust as a Filter*

The most useful way to think about trust in the EASY context is as a filter. Teams that run EASY successfully are teams that had the trust infrastructure in place before they started. Teams that struggle with EASY are, almost without exception, teams that have a trust problem that their previous methodology was papering over with process.

This is a clarifying rather than a damning observation. A Jira board with seventeen custom fields and five mandatory status transitions does not fix a trust problem. It hides it. The assignee field creates the appearance of accountability without requiring the substance of it. The due date creates the appearance of planning without requiring honest assessment of what is achievable. The status update creates the appearance of transparency without requiring the team to actually talk to each other. When EASY removes these mechanisms, whatever was hiding behind them becomes visible. That visibility is valuable, even when what it reveals is uncomfortable.

Research on high-performing teams consistently identifies psychological safety, the confidence that one can speak up, ask questions, and admit uncertainty without social penalty, as a stronger predictor of team effectiveness than individual talent or technical skill.[^1] **EASY is a methodology that functions well on psychologically safe teams and poorly on teams where people are afraid to be honest.** If you implement EASY and it does not work, the diagnosis is worth taking seriously.

*Building It*

Trust at the team level is built through consistent behavior over time, and it is built faster in some conditions than others:

- **Clear goals**: people extend more autonomy to each other when they share a clear understanding of what they are trying to accomplish
- **Outcome accountability**: holding people accountable for what ships rather than what they were assigned creates incentives for honest self-assessment rather than task completion theater
- **Tolerance for honest bad news**: teams develop communication trust when they see that raising a problem is received better than hiding it

None of these conditions are created by a project management system. They are created by leadership behavior, hiring decisions, and the accumulated culture of how a team handles difficulty. Part Three addresses each of these in turn. The methodology is the simple part. What the next chapters are about is building the organization that can run it.

---

[^1]: Edmondson, Amy C. *The Fearless Organization: Creating Psychological Safety in the Workplace for Learning, Innovation, and Growth*. Hoboken, NJ: John Wiley & Sons, 2018. Edmondson's research across industries found that psychological safety was the single strongest team-level predictor of learning and performance outcomes, outperforming factors including team composition and individual expertise.
