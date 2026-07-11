# Chapter 6: The Meeting That Replaced the Work

A standard Scrum team running by the book attends the following recurring ceremonies: 

- A daily standup 
- A sprint planning meeting at the start of each sprint 
- A sprint review at the end
- A retrospective after the review
- Regular backlog grooming sessions to keep the ticket queue organized and estimated 

In a two-week sprint, this adds up to somewhere between five and ten hours of scheduled meeting time per person, depending on team size and how tightly the ceremonies are run. For a team of eight, that is between forty and eighty person-hours of ceremony per sprint, not counting the ad hoc meetings, design discussions, and stakeholder check-ins that accumulate on top of the formal structure.

That is not a trivial number. For a mid-sized engineering organization running twenty teams, the ceremony overhead alone can consume the equivalent of several full-time employees worth of time every two weeks, time that is not spent building anything. The standard defense of this cost is that the coordination value justifies it: the meetings prevent misalignment, surface blockers early, and keep the team moving in the same direction. This defense deserves to be taken seriously, because coordination genuinely is a real problem. It also deserves to be examined critically, because the defense assumes that the ceremonies are actually solving the coordination problem they were designed for.

**The daily standup is the most instructive example, because it is the ceremony that has drifted furthest from its original purpose.** The standup was conceived as a brief synchronization point: fifteen minutes, standing up to keep it short, three questions per person. What did you do yesterday? What will you do today? Is anything blocking you? The intent was to surface blockers quickly and keep the team aware of each other's progress without the overhead of a longer meeting. It was a sensible idea for a team of humans doing complex interdependent work at roughly similar paces.

In practice, the standup has evolved into something different at most organizations. It has lengthened. It has acquired an audience of stakeholders and managers who attend to monitor rather than to coordinate. It has become a status report delivered standing up, which is a different activity than the quick synchronization it was meant to be. Studies on meeting behavior consistently find that people attend many more meetings than they find valuable, and the daily standup is one of the most frequently cited examples of a recurring meeting that participants consider low-value but feel unable to skip.[^1]

Now consider what AI does to the three standup questions. 

*Q: What did you do yesterday?*

A: I described a feature, reviewed what the AI generated, made some adjustments, and shipped it. 

*Q: What will you do today?*

A: I will direct AI to implement the next few items on the board, review the output, and move the cards to done.

*Q: Is anything blocking you?*

A: The most common blockers on modern AI-assisted teams are not coordination problems between humans; they are questions of direction and priority, which are better resolved by a five-minute conversation with the right person than by announcing them to a room of twelve.

The coordination problem the standup was designed to solve was the problem of humans working on interdependent tasks at similar speeds and needing to know what their colleagues were doing. AI assistance has changed both the speed and the nature of individual work enough that the standup's original premise no longer holds cleanly. The work is faster, the bottlenecks are different, and the information most people are sharing in a standup is less useful to their teammates than it was when every team member was doing roughly similar volumes of similar work.

The retrospective, held at the end of each sprint, has a different problem. Its purpose is process improvement: the team reflects on what went well, what didn't, and what to change in the next sprint. In principle this is a healthy practice. In reality, retrospectives at mature Scrum teams frequently produce the same observations sprint after sprint, generate action items that get added to a backlog of process improvements that never gets prioritized above feature work, and consume an hour or more of focused time from the entire team. Research on retrospective effectiveness finds that many teams report their retrospectives as repetitive and low-impact, and that action items from retrospectives have a high rate of being abandoned without implementation.[^2]

**The deeper problem with the retrospective in an AI-augmented environment is that it is designed to optimize a process that is changing too fast for the optimization cycle to keep up.** A retrospective produces conclusions about how the last sprint went, which are used to adjust the next sprint. But if AI tooling, model capability, or team prompting strategies are changing meaningfully between sprints, the conclusions from two weeks ago may already be obsolete by the time the team tries to act on them. You are tuning a system that has already moved.

Sprint planning, backlog grooming, and planning poker compound the problem by front-loading time investment in activities whose value is contingent on estimates that we have already established are unreliable. A two-hour sprint planning meeting in which the team debates whether a ticket is a three-point story or a five-point story is two hours spent producing a number that will be wrong, that will be used to generate a velocity metric that is circular, that will be reported to stakeholders as evidence of predictability that does not actually exist. The ceremony produces the appearance of rigor without the substance.

This is not an argument that people on software teams should never talk to each other. Some of the most valuable work that happens on engineering teams happens in conversation: design discussions where two people reason through a hard problem together, quick check-ins where someone shares a concern before it becomes a blocker, strategic conversations about what to build next. These conversations are worth having. What makes them worth having is that they are responsive to actual need. They happen when someone has something important to discuss, not because a calendar event fires every morning at nine-thirty.

EASY has no prescribed ceremonies because prescribed ceremonies answer the question "when do we talk" without regard to whether there is anything worth talking about. **The answer to "when do we talk" in a high-functioning team is: when we have something to say**. A card that needs clarification before someone can pull it gets clarified, on demand, between the people who need to have that conversation. A strategic question about what to build next gets discussed when the question arises. The board makes the team's current state visible to anyone who looks at it, which eliminates the standup's original information-sharing function. What remains is the actual work, moved by people who are available to move it, without the overhead of assembling everyone in a room to explain what they are doing.

**In a world where AI can complete in two hours what a developer would have spent two days on, the cost of an hour-long meeting has effectively doubled. The time is the same, the opportunity cost is not.**

---

[^1]: Rogelberg, Steven G., Cliff Scott, and John Kello. "The Science and Fiction of Meetings." *MIT Sloan Management Review* 48, no. 2 (2007): 18-21. Subsequent research by Microsoft in 2022 found that meeting time had increased by 252% since the start of the pandemic, with employees spending an average of 57.5% of their working hours in meetings or on email.

[^2]: Derby, Esther, and Diana Larsen. *Agile Retrospectives: Making Good Teams Great*. Dallas: Pragmatic Bookshelf, 2006. The gap between retrospective outputs and implemented improvements is widely acknowledged in practitioner literature; Derby and Larsen's work, while primarily prescriptive, documents the pattern extensively in its diagnostic sections.
