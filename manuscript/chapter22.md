# Chapter 22

![The Test-Driven Analysis Wheel of Pain](images/Test-Driven-Analysis-Constellation.png)

You would think that in a book like this, at some point there would be a diagram of things you haven't seen before, maybe some kind of circle or loop. Some cool new process.

Process books love circles and loops, especially colored circles with little stick figures.

I don't want to disappoint, but we did not have the budget for colored circles. Instead, all we could afford were a few dots. Even then, all we could get was grey.[^22:2]

[^22:2]: Sadly, we blew the budget on colored pyramids back in section one.

We've generalized conversations in this book, explaining how good conversations happen and why you can't replace conversations with data feeds. We've shown how to capture and store the minimum amount of information that  "remembers" what's important to you and reminds you of where and how good conversations can take place.

We've walked though several scenarios, and as we finish out small team activities and move in the next section to large teams, team-of-teams, programs, and the Meta genre -- we're found ourselves talking more and more about *action*, not information. Process. That's because in order for you to learn important things about information (Structured Analysis), I have to walk you through a lot of action that generates and uses information, even if it's just pretend action.

So what's best? What do all processes have in common? What's the best process for me? I'm looking at an A-7 scenario, dang it. Where's the little chart where I can take the scenario I have and cross-check it to find the step-by-step best process?

-sigh-

## Test-Driven Analysis Wheel

You'd think that if I were looking at trying to make some kind of generalizations about process, the obvious way would be to look at multiple examples of good processes and find similarities, right? Group them together. Look for commonalities.

Actually no. It doesn't work that way.

The reason why is that analysis is mostly mental, unspoken, and subconscious. Really the only thing I could do by cutting across and making inventories is gather together a bunch of stuff that various people have put together to do stuff -- it's all physical stuff -- most of which relies on all of that hidden, undiscovered stuff to work in one form or another. It would be more like a survey than a generalization. I'd end up with some version the measure-act-inspect loop, or DMAIC, or OODA. (All of which are wonderful loops. Big fan of OODA myself.)

This is why just about any process book has a circle or cycle in it. Once you see a cycle, it's impossible to un-see it. So we're all stuck in cycle-land whether that the best way of looking at things or not.

The actual way to work through this is to scan it all, think, then dive deep one-at-a-time, still considering the whole. Try to figure out what's going on in people's minds, not what kind of meeting they're holding. Try to build together some concepts that seem to be going on no matter what the ritual or process. Then incrementally make the situation more difficult and see if those same invisible things continue to be important. 

Doing this, you don't end up with a generalized process as much as you end up with a series of categories of questions that seem to recur over and over again, something like "categories of things your mind is doing no matter what the process". That's a different thing entirely.

There's an implication here that is interesting. A great many excellent processes might never actually outwardly do anything that looks like any of these general categories of questions. It's just that whatever you're doing, activity in those categories also happens. 

In fact, as expected, most processes that involve analysis look nothing like these categories. My money says that it might actually be counterproductive to try to create processes directly around the categories, as most of the time in analysis a direct attack results in too much paperwork and ritual and not enough, well, actual analysis. Analysis is weird in that direct attacks almost always result in suboptimal results.

Remember, this is not a book about process. If it were, it would easier. I'd just give you the process. We'd have a bunch of little charts. And cycles. With the little stick men. This book is based on what happens inside a group of people's heads when they creatively make something that never existed before.

After watching a lot of creative technical teams, it looks to me like there are five types of questions that arise during dialectics no matter what the context. All of touch on tests and testing in some way. As far as I know, they all happen simultaneously inside of people's heads as the work progresses. Or maybe in a haphazard fashion in each person. Beats me. 

So there is no loop. It's just a bunch of dots. I call it a wheel because wheels are cool. Interestingly, and this wasn't planned, it seems whatever dot you point at, dots "earlier" on the wheel have a direct impact. So it kind of turns. So it is wheel-ish. Plus I like wheels. It's my book. When you write your book, you can have cyclones, or roller-coasters or something [^22:4]

[^22:4]: I advise against pyramids. Everybody does pyramids. Earthquakes and soup would be great metaphors if you could make it work. 

Earlier in the book we were on rock-solid footing with Plato and the Greek dudes. As we move more and more into thinking-about-thinking, examining what may or may not be going on inside of people's heads, by necessity there is a lot more guesswork. I'll show you what I have. I think it's useful. I'll show you why. Be aware that this is speculative. 

There is a proud tradition with philosophers of coming up with a few good ideas -- then taking the good ideas too far. I'm no philosopher, but I'd like to do what I can to carry on the tradition.

If I manage to hit it big with any of this, I only hope one day I'll get my own toga, maybe a marble statue that I can leave for future generations. A talking statue would be incredibly cool. Maybe with a hat.

## The Dots

Each dot represents a critical group of questions that need to keep occuring.

1. What's important right now?
2. How will we know we're changing things for the better?
3. Have we completed that change?
4. What's the simplest target system we can have that still does what we want?
5. What's the simplest way of looking at the problem that makes changing the target system the easiest?

## The Types of Processes

If the dots are the general categories of questions people ask, most processes are where one dot connects to the other. This would lead to five different generic types of process-atoms, little conversations that advance analysis in one area.

1. Refinement: taking what's important and figuring out how we'll know we've done it
2. Development: taking the tests that define the positive change we want to make and making them pass 
3. Clean-up/Refactoring: Keeping all the tests passing while making the system simpler
4. Organizing/Restating: Taking what we've learned so far from engaging with the problem and re-thinking what the actual problem is 
5. Remembering/Compiling: Taking our understanding of the what the overall problem is and using that to determine what we have to do next 

Can you join dots across as well as in a circle? I don't know. That'd sure make the diagram more complicated. It'd probably use up our line budget.

## Scale Invariance

If these categories hold up, since they are about analysis in general, they would be *scale invariant*, that is, they would hold for doing tiny little jobs like TDD or giant jobs like organizing the family crazy Santa game each year.

## Question Arcs

One of the things that falls out of the diagram is the idea that whatever two nodes you are moving between, the node "prior" to those two sets up the context nicely for the work you're doing. So if you're doing development, you're making failing tests pass. But you're doing that based on what's important or not -- which is the previous dot.

If you're doing Remembering/Compiling, you're taking your simplest understanding of what you're trying to do overall and come up with what the most important things are. But you do that based on your understanding 

![](images/question-wheel.jpg)

We will continue to test out this categorization system for questions as we work through more and more complicated situations. But it's not a process. There is no cycle. It's not a wheel. Well it is a wheel, but it has no rim. You can't directly use it to go anywhere, only to evaluate other processes and your information flow to make sure you understand the types of things that happen to the model when questions pop up in any of these areas.

## Sprint Planning/"Ready for Work"

## Done/Demo 

## Retrospectives Part 1

## The Missing Meeting

Every kick-ass project I've ever been associated with had several instances where the team drastically re-imagined what the solution would look like and how they would deliver it.

I don't know if this has to be a meeting. Probably not. But being able to rework and simplify what you're doing is a critical part of intellectually owning the problem. I wouldn't trust a team that didn't do it.