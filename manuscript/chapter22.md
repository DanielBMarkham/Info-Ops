# Chapter 22

## Understanding Legacy Systems

Michael Feathers calls "legacy code" code that doesn't have any tests. The description is apt for analysis model information also. Analysis information that's not driving towards and directly associated with tests is legacy information. It exists and perhaps is critically important. There's just no validation in place to show where it is important and why. 

Data is a stream of facts. Information is data that has some sort of useful context. If I were to throw down a list of various functions I would like the computer to perform ("lookup address", "verify customer account", "sort transactions by risk") it would be data. If I were to take those same functions and stick them in at the System Abstract level associated with a Master Model, they would be information. I could cross-check the model to see why they were used. I might find various ways I could determine whether they were working correctly or not.

Because there are a lot of people who don't understand Structured Analysis, there are a million self-hatched ways of organizing stuff out there. Most of the time, people follow what I call the "book chapter" method of organization. They think of their work as a book, break it up into chapters, then decide on what goes in which chapter.

Sometimes these chapters kind of make sense. They're grouped around System Abstract functional areas in people's heads. You might see "Customer Transactions" or "Governance Auditing". People grab together a lot of things they talk about and make chapter headings.

Sometimes they don't make sense to an outsider, but make sense to the people using them. This happens when the chapter titles are more about Structure. You'll see "Back-end" as a grouping, or "Cloud Operations"

I gotta admit, "Cloud Operations" is a kick-ass title to put stuff under. I bet that team does a lot of cool stuff.

As you work more and more with legacy information systems, you'll find that there is a deep and meaningful difference between organizing by Business Behavior Abstract, future system behavior we want to implement to help folks, and any other way of doing it.

The crux of the issue is that when I'm describing and organizing things by users and their goals, I am scoping the system. If you can't show me how something helps with any of my goals, it doesn't belong in the system.

Structure is meaningless without the associated behavior and supplemental items. Show me a database and ask me if it's good? How would I know? If you told me what it was supposed to do and what rules it had to operate under, I could start figuring it out, but structure by itself is impossible to make decisions about.

So if you group things by some structural concept, like "Back-end work", I have no idea what that means. "But it's talking about all the stuff we do on the back-end!"

Yeah, I got that. But you still haven't helped me any. What stuff? Why do we do it? How would I tell whether or not it belonged there. No, not whether or not it belonged in the back-end, whether or not it belongs in the *project*. You're just telling me where something is, not giving me a clue about why it would go there or what other things might go there or be scoped out.

It's like telling me to go to town to buy groceries and put them in the back of the truck. "What do you want?" "I want stuff in the back of the truck!"

It appears to be doing something that it's not really doing.

Likewise when you organize by business function without goals? It's doing the same thing only at the business level instead of the system level. The business has organized things into various groups. You don't know how they got organized nor is it clear how that organization system impacts the rest of the work.

This is one example of the difference between "business talk" and "system talk". Nobody is a robot, so nobody can manage an entire analysis model on their own. (Although many try.) Fortunately, you don't really have to. At a business meeting, if I tell Srini to take care of the Account Reconciliation operations next month, we don't have to know exactly what it means. The words come out, Srini nods his head, and we continue the meeting.

Thank goodness it works this way. Otherwise we'd never get anything done, spending all of our time fully specifying anything we were talking about. Business works in vagaries and ambiguities. Later on, as-needed, informal analysis happens to the degree that the work can be completed.

But it's not necessarily consistent or logical. If next month I ask Medhi to handle Account Reconciliation, and he doesn't know what it is, he and I might have a completely different conversation around what I want. That's fine. As long as we reach the goals we have, the inconsistencies don't matter.

Where it becomes a problem is when it needs to translate to a formal system, like a computer program. I can't tell Srini that Account Reconciliation is one thing one month and Medhi that it's something else another month if they're both trying to write computer systems to make Account Reconciliation happen. Worse yet, if they're trying to organize people to write computer systems to make it happen.

What usually happens -- and I've seen this on at least a dozen occasions -- is that some manager somewhere ends up with a somewhat-complete list of System Realized functions that they try to map up with the business titles. Does the "MapSysExReg4" help with Account Reconciliation? That's the one we used for the RepRo project, right?

To an outsider it sounds like a bunch of gobbledygook, but it makes perfect sense to Joe Former-Tech-Guy Manager. So he sorts up all the existing functions as either being in-scope or out-of-scope. He also makes a note of new functions that might be needed.

Now that the teams have been instructed on which functions are theirs, they start to work. There's only one simple question:

How do they know if they're done?

If there's no goal, there's no test. You give me a bunch of functions to work on under the business category Account Reconciliation and two years later you might have a lot of nothing -- except bills. That doesn't mean I haven't been working. It means my work isn't connected to anything of value. It's just work under a category. We have a term for expenses that fall under particular categories but aren't directly associated with value: the term is "overhead".

The usual response is no, no. It doesn't work that way. Instead, we have a team of four-thousand QA people, all top-notch, who are double and triple-checking to make sure we're doing a good job and getting our money's worth.

Double and triple-checking what, exactly? They've got the same problem the developers have, only worse. The developers can say they're "done" with whatever they're doing at any time. The QA folks are always trying to play catch-up to figure out exactly what the heck the system is supposed to be doing. Sometimes they never figure it out.

So the common situation is finding people who have grown their own organization system. Whatever the system is, look for behavior and supplementals. Where are the tests? Where are the rules that must be true across-the-board that control how the tests are constructed?

Frankly I don't see how it's possible to organize without using behavior and supplementals without creating a lot of waste and churn. I've never seen it done...and I don't understand logically how it would work.

This means that whatever your legacy system is, if it's not around behaviors and supplementals there are going to be problems somewhere. They may not be your problems and you may be resigned to dealing with whatever you've got. The only thing you have to know is that whenever there's a legacy system involved, there's going to be pain. I am sorry.

## Legacy Meta Models

For our purposes we're going to assume that you're in a tech team without control over the various systems that keep sending you work and organizing what you do. How can Structured Analysis and EasyAM help when you have so little control over things?

In every example in this book, we've talked about walking into situations where the work arrangement was suboptimal. In each of these examples, the remedy was generally the same: try to get into a cadence of work that fixes the meta issues. If you can do that, the other stuff will come along naturally.

What you need is ATDD, and it doesn't matter if anybody else in the universe likes the idea or not. For each thing you deliver, you're going to show tests that pass to show it was done acceptably. If the work wasn't acceptable, you're going to change the tests.

Your conversations from here on out are going to be around "what tests do I need to pass for this work to be completed" Perhaps you'll just talk that way among yourselves. Hopefully you can get people outside of your team interested in talking to you in this fashion. I think they'll quickly see that it's in their best interests to do so.

That's the key first step. Without that step, no other migration activities are going to make sense. But you can do it on your own, so it's not a situation where you have to wait around for approval.

Once you start delivering in tests, the natural next step is to ask each other "I wonder how these tests might be organized?"

We, of course, already know the answer. But other folks don't, so either make them read this book or take things slowly until they figure it out. *Your ultimate goal is to use the flow of making and delivering successful tests to change Meta items and drive out the entire analysis model from the bottom-up*. I want to stress again how important it is to take your time -- due to the people aspect of this. If you dump an entire analysis model on somebody who's never seen it before, they're going to think your medication may need to be changed. If your information system is out of whack and you can't fix it, you have a Meta problem. Meta problems always have priority over everything else.

In the background, however, there's no reason you can't get organized and use the model to your advantage, no matter what the larger situation is.

## Legacy Migration

This works exactly the same as it does in greenfield: sketch out a Master Model, sketch it out again and again as you groom, then organize everything under it. The only difference is that "everything" under it might include a bunch of stuff out of your control. You'll just need to provide automated linkages.











We've talked a lot about greenfield, but what about situations where you already have dumped a ton of money and time into creating various user story and documentation systems? Do you throw all of that away?

It's not necessary. Once you get organized, I think the question you have to ask yourself is what tools are you using for what reasons.

Getting organized in a legacy situation. 



## Build Servers and Pipelines


## Legacy Migration Examples with EasyAM
automatically working with them

