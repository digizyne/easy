# Chapter 2: Built for a World That No Longer Exists

Every system is a set of assumptions in disguise. The practices, ceremonies, and tools come later, designed to serve those assumptions. When the assumptions hold, the system works. When they fail, no amount of fine-tuning the practices will fix the underlying problem.

Agile was built on assumptions that were reasonable in 2001 and remained so for most of the methodology's history. They were so reasonable that most practitioners never had to examine them. The world has changed enough that they can no longer go unexamined.

The foundational assumption: software is built by human beings, working at human speed, with human limitations, and the central challenge is coordinating those human beings effectively. This is not wrong. It is just no longer the whole picture. Consider what happens to each of Agile's major practices when AI becomes a meaningful contributor to the work.

*Story Points*

Story points were never meant to represent hours. They represent relative complexity: how difficult is this task compared to others the team has done? A five-point story is harder than a two-point story. The scale reflects the distribution of human effort across tasks of varying difficulty.

AI disrupts this at the task level. A task rated as an eight-point story might be completed in two hours when an AI coding assistant handles the research, implementation, and initial test generation. The developer's role shifts from doing the work to directing and reviewing it. Two developers on the same team, given the same ticket, can now complete it in wildly different timeframes based on nothing more than their proficiency with AI tools. **The estimate was calibrated to a baseline of human effort that no longer applies consistently.**

*Velocity*

Velocity tracks story points completed per sprint and was designed as a forecasting tool: consistent velocity makes future delivery predictable. The underlying assumption is that a team's throughput is relatively stable, because it is primarily a function of team size and composition, which change slowly.

AI destroys this stability. A new model release, a better prompt strategy, or wider adoption of AI tools can change a team's effective throughput suddenly and significantly. A team averaging forty story points per sprint might complete seventy the following sprint, not because the team changed, but because their tools did. Historical velocity becomes unreliable the moment AI becomes a meaningful contributor, because the tool's capability is not constant in the way human skill roughly is. And when AI generates substantial portions of the code those story points represent, the metric is measuring something increasingly ambiguous.

*Capacity Planning*

Capacity planning treats time as the scarce resource: calculate available person-hours, compare to estimated work, plan accordingly. It assumes that output scales roughly with human hours applied. More people, more hours, more features. It is a fundamentally industrial model.

**AI breaks the linearity of that ratio.** A team of five using AI tools effectively can outproduce a team of ten who are not. The same team might double their output next quarter when a more capable model becomes available, with no change to headcount or hours. Planning against human capacity in this environment produces the appearance of rigor while resting on a premise that is increasingly fictional.

*The Sprint*

The two-week sprint was a considered judgment: short enough to stay responsive to change, long enough to produce something worth showing. It was calibrated to a team working at human speed. When AI compresses a two-week feature into three days, the sprint becomes a waiting room. The work is done, but the process requires holding it until the sprint review.

Some teams fill the remaining time with scope expansion. Others accept the idle time as a cost of process compliance. Neither addresses the root problem: **the sprint length was chosen to match a pace of work that the best teams no longer operate at.**

These practices were thoughtful responses to real problems. The argument is not that they were poorly conceived, but that they were designed for a specific world. A 2023 study found that developers using GitHub Copilot completed coding tasks 55% faster than those working without it.[^1] A McKinsey analysis from the same year estimated that AI tools could accelerate certain software development tasks by 20 to 45 percent.[^2] These numbers will look conservative within a few years. The rest of Part One examines where the damage is most visible.

---

[^1]: Peng, Sida, et al. "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot." *arXiv preprint*, arXiv:2302.06590 (2023).

[^2]: Chui, Michael, et al. "The Economic Potential of Generative AI: The Next Productivity Frontier." McKinsey Global Institute, June 2023.
