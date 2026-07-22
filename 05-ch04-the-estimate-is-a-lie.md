# Chapter 4: The Estimate Is a Lie (And Always Was)

Ask a developer how long a task will take, and you will get one of three responses. The first is a confident number, usually rounded to a familiar interval: a day, a week, two weeks. The second is a hedge: "it depends," followed by a list of unknowns that may or may not get resolved before work begins. The third, from the most experienced developers, is a quiet sigh before the confident number, which means they know exactly how wrong their answer is about to be and have made peace with it anyway.

Software estimation has been studied extensively, and the findings are not encouraging. Researchers who have examined large samples of software projects consistently find that estimates are wrong more often than they are right, that they tend to underestimate rather than overestimate, and that increasing the sophistication of the estimation method does not reliably improve accuracy.[^1] The industry has responded to this data by developing more sophisticated estimation methods. The results have not changed.

*Why Estimates Fail*

**The reason estimates fail so consistently is not that developers are bad at math. It is that estimation is the wrong tool for the problem it is being asked to solve.** An estimate is useful when the work being estimated is well understood and has been done before in similar circumstances. Building the same house you built last year on a similar lot can be estimated with reasonable accuracy because the variables are known and the historical data is relevant. Writing software is almost never like this. The specific combination of requirements, constraints, technical context, and team composition that defines any given software task is almost always unique. There is no historical data point that corresponds exactly to the thing being estimated, which means every estimate is an extrapolation from imperfect analogies.

*How Estimates Become Commitments*

This would be a manageable problem if estimates were treated as rough guesses subject to revision as more information became available. In most organizations, they are not. Estimates harden into commitments through a process that is so familiar it often goes unnoticed. 

1) A developer gives a rough number. 
2) A manager passes that number to a stakeholder. 
3) The stakeholder builds a plan around it. 

By the time the estimate appears in a roadmap or a project timeline, it has lost its uncertainty entirely. The range has collapsed to a point. The guess has become a deadline.

Psychologists call the underlying mechanism *anchoring*: the well-documented tendency for people to rely disproportionately on the first number they encounter when making subsequent judgments.[^2] Once an estimate is stated, it anchors everyone's expectations, including the developer's. Work that would naturally take ten days becomes work that should take five because that is what was estimated, and the gap between the estimate and reality is experienced as a failure rather than as the inevitable result of guessing about something inherently uncertain.

The behavioral consequences of this are well understood by anyone who has worked on a software team under deadline pressure. Corners get cut. Testing gets abbreviated. Documentation gets deferred. Code that works gets shipped in place of code that works well. The team hits the date, or comes close enough to claim success, and the technical debt created by the sprint to the finish gets distributed across future work as invisible overhead. Deadlines do not make software better or faster to build. They make software appear to be built faster, while the real costs accumulate quietly in the background.

**The only thing due dates reliably produce is the illusion of control.** A manager who sets a due date feels, and appears to others, as if they are managing the work. They are not managing the work. They are managing the perception of the work, which is a different and significantly less valuable activity.

*The AI Factor*

Into this already-broken system, AI introduces a new and more fundamental kind of uncertainty. The estimation problem was always about predicting how long a human being would take to do something. That prediction was unreliable, but it was at least anchored to something real: the historical experience of how long similar work took similar people under similar conditions. AI assistance makes that anchor meaningless.

When a developer sits down with an AI coding assistant, the time it takes to complete a given task depends not only on the complexity of the task and the experience of the developer, but also on the following new variables:

- The quality of the developer's prompting
- The capability of the AI model being used
- How well the task maps to the model's training data
- Whether the AI's first attempt requires significant revision or ships as-is

None of these variables are captured in historical sprint data, nor can they be estimated with reference to past performance. **A team's velocity from eighteen months ago is not a useful guide to what the same team can accomplish today with AI assistance, and today's velocity will not be a useful guide to what the team can accomplish eighteen months from now when the AI tools they are using have been superseded.**

There is also the question of what, exactly, is being estimated when AI is doing a substantial portion of the work. Effort estimates in Agile were always estimates of human effort: how many hours of a developer's attention would this task require? When the answer to that question is "about two hours of prompting and review, plus however long it takes the AI to generate the code," the estimate is no longer measuring developer effort in any meaningful sense. It is measuring the end-to-end time from task start to task completion, which is a different thing, and which depends on variables that are largely outside the developer's control.

*What EASY Does Instead*

None of this argues that organizations should have no sense of when things will be finished. Customers have legitimate needs around planning. Products need to ship before they become irrelevant. Teams need some structure for prioritizing what to work on next. The argument is that due dates attached to individual tasks are a poor mechanism for providing that structure, and that they have always been a poor mechanism, and that AI has made them even poorer by destabilizing the one variable, human effort per task, on which the entire estimation apparatus depended.

EASY's answer is to separate the questions that due dates are trying to answer from the mechanism being used to answer them. The question of what matters most gets answered by the ordering of cards on the board: the most important work is at the top, and the team pulls from the top. The question of when something will be finished gets answered by finishing it, not by predicting it. **In a world where AI can take a task from not-started to done in a matter of hours, the relevant question is not "when will this be done," but "is this the right thing to be doing next," and that question has nothing to do with time estimates.**

---

[^1]: McConnell, Steve. *Software Estimation: Demystifying the Black Art*. Redmond, WA: Microsoft Press, 2006. McConnell's comprehensive review of estimation research found that software projects are underestimated by a factor of two to three on average, a finding consistent across multiple independent studies spanning several decades.

[^2]: Tversky, Amos, and Daniel Kahneman. "Judgment Under Uncertainty: Heuristics and Biases." *Science* 185, no. 4157 (1974): 1124-1131. The anchoring effect is one of the most robust findings in behavioral economics and has been replicated across a wide range of estimation tasks.
