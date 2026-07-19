# Chapter 12: What You're Not Tracking (And Why That's the Point)

One of the most common reactions people have when they first encounter EASY is not skepticism about what it includes but confusion about what it leaves out. There is no burndown chart. There are no velocity metrics. There is no cycle time measurement, no throughput graph, no capacity planning worksheet. There are no sprint reports to generate, no cumulative flow diagrams to interpret, and no quarterly roadmap to maintain in a separate system that is perpetually out of sync with the board.

For people who have spent years in Agile environments, this feels less like simplicity and more like flying blind. These metrics exist for a reason, the thinking goes, and removing them means removing visibility. If you can't measure it, you can't manage it. If you can't see the data, you can't make good decisions.

This chapter is a direct response to that concern. It examines each of the major tracking mechanisms that EASY discards, explains what problem each one was originally designed to solve, and makes the case that in an AI-augmented development environment, the cost of maintaining these systems has exceeded their practical value. This is not an argument against measurement in principle. It is an argument that these specific measurements have become poor answers to the questions they were built to address.

*Velocity*

Velocity is a measure of how many story points a team completes in a given sprint. Its purpose was always to help teams make better predictions. If a team consistently completes thirty points per sprint, and the remaining backlog contains ninety points of work, a manager can reasonably estimate that the project will take approximately three more sprints to complete. Velocity was never meant to be a performance metric, though it frequently became one. Its legitimate use was forecasting.

The problem is that velocity is only a useful forecasting tool when the relationship between story points and time is stable. Story points were always a proxy for effort, and effort was always implicitly understood to correlate with time. That correlation has come loose. When AI assistance can reduce the time required to complete a task without changing the task's inherent complexity, a five-point story might take one afternoon this sprint and three days the next, depending on how much the AI tool contributes, what kind of work it is, and how the developer chooses to approach it. The number on the ticket hasn't changed, but the relationship between that number and the time it consumes has become unreliable.

Tracking velocity under these conditions produces data that feels precise and looks authoritative but reflects a reality that no longer exists. **Teams that report velocity numbers are not lying, but they are generating a false sense of predictability**. The forecast built on that data is not a forecast; it is a story the data is telling that the work is not obligated to follow.

*Burndown Charts*

A burndown chart shows the amount of work remaining in a sprint or project plotted against time, with the expectation that the line trends downward toward zero as the deadline approaches. It was designed to give teams and stakeholders a visual signal about whether a project is on track, ahead of schedule, or at risk.

Burndown charts are particularly vulnerable to the distortions introduced by AI-augmented work. Their utility depends on work being completed at a relatively steady rate across the measurement period. When AI assistance allows a developer to knock out three tasks on Tuesday that might have taken until Friday under normal conditions, the burndown chart shows a sudden drop followed by a flat line, which looks nothing like the smooth diagonal the chart implies. The chart becomes a record of how unevenly the work happened rather than a useful forward-looking signal.

More fundamentally, burndown charts require the estimation accuracy that story points are supposed to provide, and for the reasons described above, that accuracy is increasingly difficult to achieve. **A chart built on estimates that don't reliably predict time is a chart that measures something real with a tool calibrated to measure something else**.

*Cycle Time and Throughput*

Cycle time measures how long a work item takes from the moment it is started to the moment it is completed. Throughput measures how many work items are completed in a given time period. Both are used to identify process bottlenecks: if cycle time is increasing, something in the workflow is slowing down. If throughput is declining, the team is completing fewer items than it used to.

These metrics have more merit than velocity or burndown charts, because they measure actual behavior rather than estimates. But they share a common problem with the rest of the tracking apparatus: they assume that the relationship between inputs and outputs is stable enough for historical data to predict future performance. In an environment where AI capabilities are improving quarter over quarter, a team's throughput in January is not a reliable guide to their throughput in July, not because the team has changed, but because the tools they are using have.[^1] Using cycle time data from a pre-AI period to set expectations for a post-AI period is like using 2019 fuel economy data to evaluate the performance of a 2024 electric vehicle. The categories no longer map cleanly onto each other.

There is also a subtler issue. Tracking cycle time creates pressure to optimize it, and optimizing cycle time is not always the same thing as building better software. **A team that is pressured to move cards quickly through the workflow may deprioritize careful design, thorough testing, and the kind of slow deliberation that produces maintainable systems**. The metric gets better while the output gets worse. This is Goodhart's Law in its most familiar form: when a measure becomes a target, it ceases to be a good measure.[^2]

*Capacity Planning*

Capacity planning is the practice of calculating how much work a team can take on in a given period based on the number of available person-days, accounting for vacations, meetings, and other known interruptions. It was designed to prevent overcommitment: to help teams and managers set realistic expectations about what could be accomplished and when.

The argument against capacity planning in an AI-augmented environment is the same one that runs through this entire chapter. Capacity planning works when you know, with reasonable confidence, how much effort a task will require from the humans assigned to it. **When AI can handle a significant and variable portion of the implementation work, the relationship between human hours available and tasks completable becomes difficult to establish with any precision**. A team's effective capacity is no longer simply the number of person-days multiplied by a historical productivity rate. It is a function of the work, the specific AI tools being used, the nature of the tasks, and a dozen other variables that no planning worksheet can reliably capture.

*What Replaces All of This*

The natural follow-up question is what, if not these metrics, gives a team and its leadership confidence that progress is being made and that the work is under control?

The answer is simpler than it might seem. Look at the board. Count the cards in the Done column. Look at what they represent. Talk to the people doing the work. Ask them what's moving and what isn't. These are not sophisticated techniques, but they are honest ones. They describe reality directly rather than translating it into a number that requires interpretation.

The need for elaborate metrics often grows in proportion to the distance between decision-makers and the work being done. When a manager can see the code, read the pull requests, and talk to the developers, they do not need a velocity chart to understand whether the team is productive. The chart becomes necessary when visibility is lost and a proxy is needed. EASY does not solve that organizational problem, but it also does not paper over it with data that creates the appearance of visibility without the substance.

**What EASY asks of teams and their leadership is to accept that some uncertainty is irreducible and that the right response to that uncertainty is not more measurement but better trust, clearer goals, and more direct communication**. The goal was never to generate accurate metrics. The goal was always to ship good software. Keeping those two things from being confused with each other is one of the more important things a simple board can do.

---

[^1]: For evidence on the pace of AI productivity gains in software development, see Peng et al. (2023) and Chui et al. (2023), cited in Chapter 2.

[^2]: The principle originates with Charles Goodhart's 1975 paper on monetary policy. The formulation most commonly quoted today, "when a measure becomes a target, it ceases to be a good measure," is a paraphrase attributed to the anthropologist Marilyn Strathern. See Chapter 5 for the full citation.
