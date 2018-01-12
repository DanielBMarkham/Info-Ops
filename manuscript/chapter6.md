# Chapter 6

In 2004 I worked on a secret bom for the Department of Defense.

It's not something I talk about a lot. It was a long time ago. My country needed me.

A DoD agency called me in to work on replacing a set of critical systems that all worked together with one system that would be easier to modify and maintain.

As a software architect, I didn't know what to expect. Clients have all sorts of ideas about how to start off major new efforts. Most times they place so many constraints on the system before they even figure out what it's supposed to do that it's doomed to failure.

I was asked what I needed. "A big open space where we can work side-by-side, a couple of months or so, and people who have a lot of experience in the various ways these other systems work."

Monday morning when I showed up, they sent me to an abandoned Food Lion, which is a grocery store chain in the U.S. The agency had rented out the entire store, and when I walked in there were about dozen people waiting for me in the empty building.

"Who are you guys?"

"We're the experts you requested for two months. Are you ready to go now?"

I looked around. All of these people were staring at me. So we blocked off a little theater where we could set up a projector, then gathered around some chairs. I brought up notepad and a drawing tool on the screen and started asking questions.

The entire gig consisted of all of us in that room asking questions of one another and writing down the conclusions we reached. We also brought in folks from other parts of the agency and asked them questions.

Initially, our quesions focused around what the current various systems did, but we also had to talk about what the new system would do.

But wait, that's two completely different things, right?

## Temporal Indicators

Our last group of tags are called **Temporal Indicators**. Since I build software for people, most of the time our discussions are around what they want in the future. But a few times in my career I've had to spend time talking about how things \were in the past -- or how they are currently.

The Temporal Indicators I've used for those situations are **Was, As-Is, and To-Be**

Certain situations might have a need for other indicators. I don't know. These have worked for me and I've never seen any others used.

![Analysis Bingo with Temporal Indicators added. Most all you'll need are those boxes at the bottom](images/full-analysis-bingo.png)

The grid's a great way of looking at the tagging system. Everything goes into one of the boxes. We need to remember, however, that there is a pyramid of parents to children inside of each box. There's also a pyramid relationship that runs along this path Business Abstract -> Business Realized -> System Abstract -> System Realized

I'm going to use pyrmids from here on out. The purpose of our grid is to show that the tagging system itself is really simple to use. Once things are tagged, where it gets interesting (and powerful) is in those parent-child relationships and the way things in the different buckets interact.

![](images/bucket-pyramids.png)

The project with the DoD went very well. The customer was concerned that our super user group would disagree on critical components of the new system. That was a valid concern. They did disagree. But what we did was first talk about the "as-is" situation, outlining all the various ways the different units went through their job without respect for technology -- the **Business Applied As-is** Behaviors, Structures, and Supplementals.

Everybody had a say in describing what world they came from and what was important in that world. Once I had all of the **Business Applied As-Is** items in place, I asked a simple question: "What sort of generic things are true across all of these instances?"

The group was then able to describe generic behaviors, structures, and supplementals that would have to be true in the upcoming system. We were able to work at the **Business Abstract To-Be** level without any problems. From there, we took that agreement and did all kinds of other cool things we'll talk about later.

What was the agency? What was the mission?

I was working for the Defense Commissary Agency. They run a series of grocery stores all over the world supporting the troops. As part of our work back then, I had to sign a non-disclosure agreement, of course. We also created something called a "Business Object Model", or "BOM"

Yep, I worked on a secret bom for the Defense Department. The bom involved green beans.

