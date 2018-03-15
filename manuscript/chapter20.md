# Chapter 20

Congratulations! You've just received a large grant from a well-known charity to write software to support oppossum flying schools. Flying squirrels get all the good press, and the radical fringe group "Opossums United Curicculum Help (OUCH!)" wants somebody to develop a computer program to help those brave folk around the world who are teaching opossums to fly. They are too often forgotten. Have you ever seen a fundraiser for oppossum trainers? Ever see a flying opossum? See?

Along with the grant came a first-class ticket to Hooterville, Inidana, home of Peter Principal's Possum Pilot School, school for possums wanting to break free of the usual midnight snack around the cat bowl and launch themselves into the void.

And you have a team of three! Woot! It's about time you got some help around here.

As you walk through the gates and onto hallowed ground, a plaque welcomes you, reminding you of the terrible price of failure.

![](images/opossum-mypossum.png)

When you meet Peter, owner of the school, the first thing you ask him is if he and your team can just work side-by-side for a few weeks. You'll help him with the possum pilot preparations, he can help you with the coding. This would create an instant feedback loop, eliminate any kind of analysis or backlog, and cut the crap down to the minimum-needed to get this software written. Also I would get to skip writing the rest of this chapter.

This does not work for him. The demands of opossum organizations are oppressive and obstinate, such that we'll have to set up some kind of schedule. In addition, there are other possum schools that need to use the software. Peter isn't a customer, rather, he's not *all* of our customers. He's just a guy to help us understand the needs of possum people.

-sigh-

Ok. So who *are* the customers? Where are they? What do they look like? It's good you're doing analysis because you guys have a ton of questions. You look up the number to the OUCH! people and give them a call.

As it turns out, those headquarters maroons don't even want software right now. All they want is you to come back in a month or two and pitch them on what software *might* look like. Ouch!

You've read this book, so you know that analysis work without a test is breaking the rules. How are you supposed to know that the model is developed enough without a test? You could stop after five minutes. You could take five years. This is the crux of the problem with analysis paralysis. No tests, no end in sight.

How about if you guys built a *prototype* application while talking to Peter? It'll take the same amount of time either way, and you'd feel much better to have something to show them.

They're okay with that. Hanging up the phone, you have two goals in mind for your work:

1. Understand the world of opossum pilot training enough to propose and explain a software app, and 
2. Do that by building a prototype app that covers some of Peter's most pressing needs

The team spends an hour with Peter asking whatever questions come to mind. As he answers, the team asks follow-up questions, bouncing from bucket to bucket and trying to stay at the Business Abstract level (in their heads. Let's not bother Pete with Structured Analysis. He's got possum work to do.) 

In fact, whenever Pete wandered into System Realized stuff, as real humans are wont to do, the team took especially careful notes, looked as sympathetic as they could -- then tried to capture what Business Abstract Behavior or Supplementals Pete was instantiating. The actual stuff he said at that level stayed in their heads but did not go in the notes. (Why? Because if we don't understand why we're helping Pete, Pete's world, we're never going to understand all the thousands of other possum trainers out there like Pete.)

Pete doesn't know it, but Pete is training us to think like Pete. That's the real goal of the entire grant: know these possum flight trainers well enough to be able to anticipate their needs. (That's the goal of any technology development effort.)

Then you all go back to the hotel. Time for some grooming!

The first thing you do is compare notes, agree on what you understand, then run the final version through EasyAM. The meeting with Pete was step 1 of grooming, "introducing new information for the team to consider". 

![](images/chapter20-initialnotes.png)

Our agreed-upon notes covers all of the top and most of the second section of the Analysis Survey. Those sections set the stage for whatever activity is going to happen.

![](images/chapter20-initialucm.jpg)

![](images/chapter20-initialdm.jpg)

Step 2, "synchronizing the analysis model", was handled just by everybody taking their notes and agreeing on one version for EasyAM. If you had already had stuff written down, you would have to have everybody agree with one another, then agree with your previous notes. Otherwise something's gotta change somewhere.

Step 3 is cleaning up the backlog to make it manageable. There is no backlog! So let's throw a few things on there tomorrow for Pete to look at.

Here's how to intially order a backlog with no Product Owner input: look at all the domain objects. Sort them by how important they've been to the conversation so far, like so:

* Number of connections
* Number of arrows leaving 
* Number of attributes identified

So for our model, we have:

* Teacher
* School
* Administrator
* Training Period
* Possum
* Course
* Tribe
* Catapult

Possum and course were tied, so we just picked one.

Now, for each domain entity, walk through the behaviors and list the ones that affect it. To do that, we "walk the model", going down the behavior list and pointing out domain entities while describing what happens.

For "gather possums", we go to the woods and, well, gather possums. The word "woods" is unlikely to show up anywhere else so it's not important. So that behavior right now only has one noun, "possum", along with the actor, "administrator". Next to "administrator" and "possum", we add "gather possums"

Next one is "organize possums into tribes". It's like the first one. For all we know right now, the only nouns it uses is "administrator" and "tribe". So next to administrator and tribe we add "organize possums into tribes"

Next is "administer flying tests". Next to "administrator" we add "administer flying tests"

Wait! "Test" seems like an important word. We'll be talking about that a lot. But it's not in our domain model! Yikes! We make a note to add it later (Or add it right away. You can do it either way) And what does the test actually check, anyway? It checks how much of the training material has been learned by the possum, right? So --- where's "training material". That's an important phrase. Don't see it anywhere either.

Well frack. This is getting out of hand. So we make a note to add "training material" and continue on.

"Assign possums to classes" affects possums, course, teacher, training period, administrator

Wait a minute. We catch these possums in the woods, right? So how do we know that they're eligible for classes? Don't we have to enroll them?

Geesh. Ok. So add "Enroll possums into school" to our list of things to add 

Now we have "launch possums from catapults" which involves a teacher during a training period taking a possum and shooting him into space using a catapult. 

"Clean possums" affects only the teacher and the possum involved

"Create training material" is where a teacher creates training material for a course which needs to be approved by an administrator

"Create flying tests" uses the teacher, training material, course, and administrator again

* Teacher: gather possums, organize possums into tribes, assign possums to classes, launch possums from catapults, clean possums, create training material, create flying tests
* School: enroll possums into school (which we haven't added yet)
* Administrator: gather possums, organize possums into tribes, administer flying tests, assign possums to classes, create training material, create flying tests
* Training Period: assign possums to classes, launch possums from catapults
* Possum: gather possums, organize possums into tribes, assign possums to classes, launch possums from catapults, clean possums
* Course: assign possums to classes, create training material, create flying tests
* Tribe: assign possums to tribes
* Catapult: launch possums from catapults

We've sketched out a list of nouns by importance (Remember, the domain model is a visual hierarchical dictionary). Then we've listed out the behaviors that affect them.

But we have new nouns! New behaviors! Shouldn't we re-do the list?

No. We should not. We're grooming. We're not writing a spec. If this takes more than a few minutes we're spending too much time on it. Our goal here is to "gain agreement that enough has been described to create a failing test at some lower level." In other words, do we have enough to create an ordered list of behaviors we might want to test?

We do. "Assign possums to classes" both appears associated with our most important noun ("Teacher", for now) and with the most other nouns (4). Second place looks like "Create Flying Tests" which has 4 nouns total. Third place is "Create training material", which also impacts our most important noun and hits on 3 nouns total. 

Fourth place? Who cares about fourth place? Second and third place were probably doing too much. Just throw stuff in there. So now we have a prioritized Master Backlog.

* Assign Possums To Classes
* Launch Possums From Catapults
* Create Training Material
* Create Flying Tests
* Create Training Material
* Gather Possums
* Organize Possums Into Tribes
* Clean Possums

If you've taken any sort of backlogs course in the past, you're probably yelling, "Why would we want to create a backlog without a customer or product owner present?"

***Because we want to be wrong***

We want a test. Analysis happens naturally. In any given week a good team is probably going through 50 grooming cycles, most of them informal. In a lot of ways, it doesn't matter what we put down here as much as it matters that we have something to continue talking about with the customer. We have a test that could pass or fail.

Since we haven't quite spent an hour yet at the hotel, and since we can use what we have in the model to make more tests, we sketch out some screens (System Realized Structure) to show to Pete tomorrow and get his feedback.

Then we go back and add our new items to EasyAM, printing out the new diagrams.

![](images/chapter20-ucm2.jpg)

![](images/chapter20-dm2.jpg)

## Grooming Examples With EasyAM

Pointing
Splitting
Bug dump
Feature request


1. You are not allowed to have any important conversations unless it's to validate items already in the analysis (shared mental) model
2. You are not allowed to add things to the model unless it answers a relevant question or fixes a failing test at the current level 
3. You stop adding things to the model as soon as there is agreement that enough has been described to create a failing important test at some lower level

The ordering of tests by importance is called the backlog queue


