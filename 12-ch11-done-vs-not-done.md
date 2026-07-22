# Chapter 11: The Binary Beauty of Done vs. Not Done

There is a phrase that haunts every software project: "ninety percent done."

It appears in status meetings and roadmap updates and it gets passed up the chain to stakeholders who accept it as meaningful information, not realizing that it is almost always a polite fiction. Work that is ninety percent done is not ninety percent of anything. It is work that has been started and not finished, dressed in a number to suggest progress where none can be confirmed. The remaining ten percent, in practice, has a way of containing everything that is actually hard about the task: 
- Edge cases
- Integration problems
- Review feedback
- Discovered requirements that weren't in the original description 

"Ninety percent done" is another way of saying "we have no idea when this will be finished, but we needed something to say."

**The Done/Not Done binary eliminates this class of ambiguity entirely.** There is no "ninety percent" or "mostly done" or "functionally complete" or "just needs polish." A card either represents work that exists in the world in the form it was intended to exist, or it represents work that does not yet exist in that form. These are the only two states that a card can be in, and the discipline of maintaining that binary is one of the most practically valuable things about EASY.

This is not merely a philosophical preference for simplicity. The binary produces specific, observable benefits in how teams work. When there is no intermediate state, work does not accumulate in ambiguous limbo. A developer working on a card is either finishing it or discovering that it needs to be broken into smaller cards because the scope is larger than the description implied. Those are both useful outcomes. What is not useful is the card sitting in a state called "In Progress" for a week while the developer works on other things in parallel, returning to it intermittently, never quite finishing it, and updating its status to "seventy percent" in advance of a stakeholder review. That pattern is common in complex ticketing systems and almost impossible in EASY, because EASY offers nowhere for the pattern to live.

*Defining Done*

The binary also creates useful clarity about what "done" actually means, which is a question that deserves more attention than it usually gets. Done does not mean:

- The code is written
- The pull request is open
- It works on my machine

Done means the work described on the card exists in the state in which it was intended to exist, and is available to the people it was built for. In most software contexts, that means the code is reviewed, merged, deployed, and functioning in its intended environment. The card can be moved to Done when the thing it describes is real.

**Defining done this way shifts the emphasis from activity to outcome, which is precisely the shift that EASY is designed to produce.** A developer who thinks of done as "I finished coding" will have a very different relationship with a card than a developer who thinks of done as "this thing now exists in the world." The second definition keeps the work honest. It prevents the premature satisfaction of closing a ticket before the thing it describes actually exists in the intended form.

Some teams find this definition challenging because it puts deployment and review inside the scope of "done," which means cards cannot be moved until those steps are complete. This is by design. If deployment is slow or review cycles are long, the EASY board will make those bottlenecks immediately visible in a way that a more complex ticketing system often obscures. Cards that cannot reach Done because deployment takes three days are not a board problem. They are an infrastructure problem, and making that problem visible is more valuable than hiding it behind an intermediate "Deployed, Pending Verification" column.

*Who Makes the Judgment*

The question of who makes the Done judgment returns here, because it matters more than it might seem. In a world where AI generates substantial portions of the code, documentation, and tests associated with a piece of work, the Done judgment cannot be delegated to the AI. The AI can tell you whether its output compiles and passes the tests it was asked to write. It cannot tell you whether the thing you wanted to build has been built to your satisfaction, whether it handles the edge cases your users will encounter, or whether it reflects the design intent that was in your head when you wrote the card. Those judgments require a human being who understands the intent.

This is one of the reasons the outcome-description format for cards matters so much. A card written as an outcome gives the person reviewing it a clear target for the Done judgment. Either the registration form validates email addresses as described, or it does not. Either the dashboard loads in under two seconds, or it does not. Either the user can complete the checkout flow without errors, or they cannot. These are questions a human being can answer by looking at the thing that was built, and that answer is the only thing that moves the card.

**Done is not a technicality. It is a commitment that the work the card described now exists in the world.** Everything in EASY is organized around producing that state as efficiently as possible and representing it as honestly as possible. The binary is not a simplification of something more complex. It is the most accurate representation of the only thing that ultimately matters: either the thing exists, or it doesn't yet.

