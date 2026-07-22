# Chapter 10: The Board

The EASY board has two columns.

The left column is called Not Done. It contains every card that represents work the team has committed to doing but has not yet finished. Cards might be ordered from top to bottom by priority, they might not. EASY doesn't mandate or care how they are ordered.

The right column is called Done. When a card's work is complete, it moves there. It stays there. That is the entirety of the board's structure.

**The board is not a reporting tool, a management dashboard, or a visualization of team capacity. It is a shared map of what the team is navigating toward.** Anyone who looks at it can answer two questions immediately: 

1. What does the team still need to do?
2. What have they already done?

Those are the only two questions the board is designed to answer, and it answers them accurately and without maintenance overhead, because the only action required to keep it current is moving a card from left to right when work is complete.

*Why No "In Progress" Column*

The most common question about this structure is why there is no column for work that is currently in progress. The question is reasonable, and it deserves a direct answer.

The "In Progress" column exists in most Kanban implementations to make visible the work that has been started but not yet finished, on the theory that knowing what is actively being worked on helps the team avoid duplication and allows managers to see where effort is currently concentrated. These are real concerns, and in a pre-AI team working at human pace they justified the column's existence. Work that takes three to five days to complete will genuinely occupy a visible "in progress" state for most of its life, and surfacing that state provides useful information to the people coordinating around it.

AI changes this calculus in a specific and important way. **When a substantial portion of work moves from start to done within a single working session, the "In Progress" state lasts hours rather than days, and a column that represents it is stale almost as soon as it is updated.** A card moved to "In Progress" at nine in the morning by a developer using AI assistance may well be in the Done column before lunch. The intermediate state is real but so brief that tracking it imposes more overhead than the information it provides is worth. Whoever finishes the work will move the card to Done, and anyone who needs to know what is being worked on can ask the person doing the work. The board does not need to represent a state that exists for only a few hours, because the board's job is to show what is done and what is not.

There is also a subtler reason to resist the "In Progress" column. Any intermediate state between Not Done and Done is an invitation to park work there. Teams that have an "In Progress" column develop a habit, often unconscious, of moving cards into it at the start of a work session and leaving them there when the session ends without the work being finished. The column absorbs cards that have started but not completed, which is a softer version of the same problem it was supposed to solve. Work in the "In Progress" column is still not done, but it has been moved to a state that looks like progress, which reduces the psychological pressure to finish it. EASY removes this escape valve. A card is either done or it is not. There is no resting state in the middle.

*Why No "Blocked" State*

The "Blocked" state deserves similar treatment, because it comes up almost as frequently. Teams accustomed to more complex boards often want a way to flag cards that cannot move forward because of an external dependency or an unresolved question. The impulse is understandable: if a card is waiting on something outside the team's control, it seems wrong to leave it sitting in the Not Done column as though it were available to be worked on.

EASY's position on blocked work is that blocking is a communication problem, not a board-state problem. When work is blocked, the right response is to communicate with whoever can unblock it, not to create a visual category for the stuck state. A card that is blocked stays in the Not Done column, and the team leader coordinates with the necessary people to remove the blocker. The board does not need to represent blocking because the board's job is to show what is done and what is not. **Blocking is a temporary condition that belongs in conversation, not in the data model.**
