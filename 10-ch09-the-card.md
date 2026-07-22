# Chapter 9: The Card (And Only the Card)

The atomic unit of EASY is a card. Everything in the system flows from it, and understanding what a card is, and what it deliberately is not, is the bulk of understanding the methodology.

A card has one thing on it: a description of the work to be done. That description should be specific enough that any member of the team can read it and understand what the world looks like when the work is complete. It should be concise enough to be grasped quickly. It should be written in terms of outcomes rather than instructions, describing what needs to exist rather than the steps to make it exist. Beyond the description, a card in EASY has nothing else.

*The Absences*

A card in EASY contains only a description of work. Specifically, a card omits:

- Assignee
- Due date
- Story points
- Priority field
- Labels
- Epic link
- Sprint association
- Status field (beyond the column it occupies)

Each omission is deliberate:

- **No assignee** keeps work in a shared pool that any available team member can pull from. It removes the dedication queue problem and reflects the reality that in an AI-assisted team, individual ownership of a unit of work has become increasingly ambiguous.
- **No due date** removes the anchoring effect that turns estimates into commitments and pressures teams to cut quality to hit a date.
- **No story points** removes a measurement calibrated to human effort that is now unreliable as AI assistance varies dramatically from task to task. It also eliminates the estimation ceremonies and velocity tracking that story points require.
- **No labels, epic links, or sprint associations** removes taxonomy overhead that exists primarily for reporting rather than for helping the team do work.

What remains when all of that is stripped away is a unit of intent: a statement that something needs to exist in the world that does not yet. **A card is not a task description. It is a gap between current reality and intended reality, expressed as briefly as possible.**

*Writing Effective Cards*

This distinction matters in practice. A task description says "write a function that validates email addresses." An outcome description says "email address validation is in place on the registration form." The first describes an action. The second describes a state of the world. The first can be completed without the problem being solved if the function is written but never wired up. The second cannot be moved to Done until the thing that needs to exist actually exists and works.

Writing cards as outcome descriptions rather than task descriptions has a secondary benefit in an AI-assisted environment: it gives AI tools better context. When a developer hands a card to an AI coding assistant, a description of the desired outcome is more useful than a description of the steps to achieve it, because the AI can determine the steps. What it cannot determine is the goal. The card, written as an outcome, carries that goal clearly.

The question of how much detail to include in a card description is one that teams calibrate over time, but the guiding principle is simple: include enough information that the person pulling the card can make a confident judgment about whether the work is done. If the description is so brief that someone completing it would have to guess at the acceptance criteria, it needs more detail. If it is so long that it is prescribing implementation decisions that should be left to the person doing the work, it has too much.

*Card Size in the AI Era*

**The size of a card matters, and AI has shifted what the right size looks like.** Before widespread AI assistance, a card that described two or three days of focused developer work was a reasonable unit. Today, with AI assistance compressing many development tasks significantly, a card describing two or three days of pre-AI work might be completed in a few hours. This does not mean cards need to be broken into smaller pieces automatically. It means the team should calibrate card size to what can be taken from start to done within a short, continuous work session, which is now often shorter than it used to be. A card that can be completed in an afternoon is about the right size. A card that will require multiple sessions across multiple days is probably better split into two or three smaller cards.

This calibration is not something EASY mandates or enforces with rules. It is a judgment the team develops through practice, in the same way a well-functioning kitchen develops a sense of how large to cut vegetables without measuring each piece. The goal is cards that move. A backlog full of cards that never seem to finish is usually a backlog full of cards that are too large, too vague, or both.

The card is the entire data model of EASY. Every other element of the system, the board, the backlog, the ordering, the done column, is just a way of organizing cards and answering the question about each one: is it done?

