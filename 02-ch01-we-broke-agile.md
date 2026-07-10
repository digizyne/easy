# Part One: The Agile Trap

# Chapter 1: We Broke Agile

In February of 2001, seventeen software developers met at a ski resort in Snowbird, Utah. They were frustrated. The dominant approach to building software at the time, characterized by detailed upfront planning, rigid requirements documents, and multi-year delivery timelines, was failing projects at a spectacular rate. The Standish Group's CHAOS Report from 1994 had found that 31% of software projects were cancelled outright before completion, and 53% overran their budgets by nearly double.[^1] The industry had a serious problem, and these seventeen people thought they knew why.

The result of that Snowbird meeting was the Agile Manifesto: sixty-eight words of principles and four value statements. The whole thing fits on a single page with room to spare, and that brevity was intentional. Agile was never meant to be a complicated system. It was meant to be a corrective, a course adjustment away from the slow, brittle, plan-heavy approach that was producing so many failures.

The manifesto's values held up well. Its principles were straightforward and sensible:

- Favor working software over documentation
- Welcome changing requirements even late in development
- Deliver frequently
- Trust the people doing the work

These weren't just reactions against waterfall's rigidity; they were a coherent philosophy about how creative, knowledge-intensive work actually gets done. Build a little, learn a little, adjust, and repeat. Don't plan so far ahead that your plans become irrelevant before you execute them. Let the people closest to the work make decisions about the work.

For a while, this approach delivered real results. Teams that adopted Agile practices in the early-to-mid 2000s genuinely shipped faster. They responded better to customer feedback. They had fewer catastrophic surprises at the end of long development cycles. The philosophy was sound, and early implementations were close enough to the original intent that the benefits were tangible and measurable.

The problems came later, as Agile grew from a philosophy into an industry. Certifications, frameworks, and methodologies began to multiply throughout the 2000s and into the 2010s. Scrum was codified into a formal guide, and that guide grew with each successive revision. SAFe, the Scaled Agile Framework, emerged as an answer to how large organizations could adopt Agile principles at scale, and the answer turned out to involve a great deal of additional process. SAFe's framework diagram resembles a circuit board. It defines roles that most software professionals have never encountered, and it includes ceremonies specifically designed to coordinate other ceremonies.

**This is where Agile began to contradict itself in a fundamental way**. The original manifesto explicitly favored "individuals and interactions over processes and tools," but within a decade, Agile had become primarily a system of processes and tools. Jira launched in 2002 and by the 2010s had become the de facto project management system for software teams worldwide. With it came configurable workflows, custom ticket fields, dependency graphs, roadmap views, and portfolio management dashboards. The tool that was supposed to serve the process gradually became the thing teams organized their working days around.

The ceremony burden expanded in parallel. Sprint planning meetings now routinely run two to four hours. Retrospectives generate action items that get added to backlogs that are never fully prioritized. Backlog grooming, a ceremony literally named after the act of maintaining the maintenance system, became a recurring calendar event at thousands of companies. Scrum Masters emerged as a dedicated role whose primary function is to facilitate the ceremonies themselves rather than to contribute directly to the work being done.

There is an uncomfortable irony in all of this. A discipline born from frustration with too much process has, in its maturity, produced more overhead than many of the systems it was designed to replace. And the cost is not abstract. Research consistently shows that software developers average fewer than three hours of uninterrupted coding time per day.[^2] A study by Atlassian, the company that makes Jira, found that employees consider 60% of their meetings to be unnecessary.[^3] These are real hours belonging to real people, spent on coordination rather than creation.

For years, the argument in defense of this overhead was that the coordination was worth the cost. When work is complex and humans are doing all of it, you need systems to ensure everyone is aligned, to catch blockers early, and to prevent individual contributors from marching in divergent directions. That argument had merit when it was made, because the underlying assumption was reasonable: the people in the room are the ones doing the work, they are doing it at a pace constrained by human capacity, and managing their coordination is a legitimate challenge that justifies dedicated time and tooling.

**That assumption is no longer reliable, and its erosion changes the calculation entirely**. AI coding assistants are now generating production code. AI tools are drafting product requirements, writing test suites, and documenting APIs. The tasks that once occupied a developer for a full day can now be completed in a few hours with AI assistance. Work that previously required a week can be done in a day. This compression is not speculative; it is happening on software teams right now, and it is accelerating with each passing quarter.

Consider what that compression does to your process overhead. If real development work has shrunk from six hours to two hours to produce equivalent output, but the two hours of daily meetings and half an hour of ticket updates remain constant, the overhead has gone from roughly a quarter of a developer's day to more than half. The ceremony that was once a supporting structure for the work has become larger than the work itself.

The Agile Manifesto was written in 2001. Jira launched in 2002. The Scrum practices most teams follow today were largely codified by 2010. GitHub Copilot went generally available in 2022, and AI coding capability has improved dramatically in every year since. These tools have fundamentally changed the pace and nature of software development, but they have not changed how most teams manage it. The methodology was built for a world where humans did all the work, all the work took a predictable amount of time, and the central challenge was coordinating many people across many long-running tasks. That world has not disappeared, but it is no longer the whole picture, and in many organizations it is no longer even the dominant one.

The chapters that follow examine what happens to specific Agile practices when you hold them up against this new reality. Some dissolve immediately under scrutiny. Others reveal themselves to be answers to problems that AI has quietly solved. A few survive, and those survivors form the foundation of something leaner and more honest about how software is actually built today.

---

[^1]: The Standish Group, *CHAOS Report* (West Yarmouth, MA: The Standish Group International, 1994).

[^2]: GitLab, *2021 Global DevSecOps Survey* (San Francisco: GitLab Inc., 2021). Available at gitlab.com/developer-survey.

[^3]: Atlassian, "You Waste a Lot of Time at Work," Atlassian.com, accessed 2026. Available at atlassian.com/time-wasting-at-work-infographic.
