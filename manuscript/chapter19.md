# Chapter 19

![](images/tda2.jpg)

Just to get everybody caught up, a backlog is a series of partially-constructed tests. We make those tests by combining Behavior To-Be and various Supplementals To-Be. We don't develop the tests all at once, instead, we continue to mature the analysis model and then pick off pieces to make into tests once we get close to when we want to use them. 

Tasks are to-do items. They may be associated with tests -- or not. They may be just things we'd like to do one day. They may be tremendously valuable things that must happen right away! Or things we'd like to do one day. Tasks may be *associated* with tests, but they have no tests directly tied to them. There's no test you perform to see if a task is done aside from just looking at something. Did you wash the car? I did! (Looks at car). I see that. Thanks!

You can't tie tasks to goals/tests without mentally defining what you want it to look like and how it's built. At that point, all creative work stops. Any analysis work is done. Goals/tests created from the analysis model define value. Tasks define *activity*, not *value*.

Tasks do not go in the backlog. A list of tasks is just a to-do list. Tasks are fine and necessary, they're just not related to what you're trying to change as much as they describe what you are doing. In many cases there's no match between the two. The worst thing is that tasks can appear to be providing value when in fact they're introducing tons of friction and waste into the system. By breaking things into tasks, you end Analysis, since you're assuming the solution and how you're reaching it is both known and fixed. 

Tasks are good and necessary in other areas, though. Set aside time for to-do items everyday. Put post-its on your monitor.[^19-1] There are tons of ways to keep track of your tasks. It's just that the backlog isn't one of them. Because of all of that, in general, breaking down creative work into written tasks should be avoided.[^19-0]

[^19-1]: When I develop software for myself my entire tracking system consists of post-its on my monitor. On the left is to-do, on the right is completed. At the bottom are things I need to consider. The entire model exists in my head, and the reason I refuse to use any more structure than that is that if I can't see it, it doesn't exist. I want my mind constantly going through the analysis model and how it relates to the work-in-progress. Otherwise, if I put things in a doc somewhere, for me it's just a formal way of forgetting about them.

[^19-0]: Most everybody will have examples of where they had a creative job, broke it into tasks, and everything worked out fine. In most all of these cases, that's because there are only one or two people involved, the task list isn't considered written in stone, and everyone involved is actively challenging the shared mental model with one another as they go along. That's a wonderful thing when it happens, but it only works in extremely tiny and constrained situations. You'd be fool or idiot to try it in the commercial world. Even in those isolated environments, it's as likely to fail as succeed.

The same can not be said of breaking down big tasks into smaller tasks in a non-creative, factory-like environment where value discovery is completely off-the-table.

**The backlog isn't about stuff you're going to do. It's about ways you're going to change the target system.**

Ideally you wouldn't do anything and change the target system to provide fabulous wealth and we're all living on tropical islands drinking those drinks with little umbrellas in them. Worst-case, you have some to-do list from hell that you call a backlog and everybody far too much work than they ever could get done and the target system doesn't change at all.

## How NOT to do Backlog Grooming

Require a large group to attend. Only have it once a month or so, and make sure the group that is attending never see each other much during the day. (This will provide for an incredible amount of cross-talk and make it difficult to stay focused). Use a projector in a darkened room, especially after lunch, because who doesn't like projectors in a dark room after a big meal?

Once everybody is assembled, bring up a big list of items on an electronic tool, preferably all prefixed with some impenetrable code that you use as a moniker. "First up is CS743183 dash seven. Who can forget that one?"

Ask a bunch of questions that are related to whatever process you are doing instead of the nature of the work. "How many points for 'Reverse polarity on the deflector array?'", and "Has the TPS cover sheet been completed for this?"

Make everybody wait while you click around through some interface.

Never talk about the overall scope of work, only tiny items in a large, seemingly-endless list. Bonus points if you can spend a large chunk of time discussing some System Realized issue that few in the room care about or can engage in.

As you go along, never clean up. Instead, just keep incrementally adding stuff here and there. Don't refactor 17 items into 3, instead, keep adding new items and keep adding a lot detail for existing items. Sometimes you'll copy and paste, sometimes you'll re-type things, only using different terms. The important thing is that over time it just keeps getting bigger and bigger. It's the Backlog Blob that ate Cincinnati!

Hold it a day or two before sprint close, so that it people will be sitting there worrying about completing the rest of their work.

Do this enough times and you could be brought up on war crimes. You also may get a promotion. Either is equally likely. I wouldn't risk it if I were you. Trust me.

## Backlog grooming/refinement

![](images/Backlog-Refinement.png)

Good grooming does five things:

1. Introduce new information
2. Synchronize the Model
3. Clean up the backlog
4. Verify we're ready for the next bit of work
5. Tease out the best way the entire model might be delivered

Meanwhile, of course, the good, honest questioning, the dialectic continues.

The actual creation and execution of the tests happens somewhere else.[^19-3]

[^19-3]: Although with more automation, I'm beginning to see teams complete fully-specified and executing tests during this time.

Grooming is what we did in the deck example every time we went back home and got organized for another conversation. "What will it do when it's done? What's important right now? What's it have to start doing next?" would be a good slogan for grooming.

Grooming is also what happened as we played with a physical model of the deck with the customer, only it was informal grooming. (The best and fastest kind, by a couple orders of magnitude.)

Ideally grooming happens continuously. There's no reason it has to be a separate meeting or big formal event. But many times we don't have time to get organized and leave things in a mess. Stuff gets thrown in notes that should be master model items. Questions are stuck in the wrong place. There's a new supplemental that we haven't had time to talk about. 

Most importantly, not everybody on the team is capable of cleaning up and getting organized, which means that keeping things neat ends up bottle-necking through the people who know how to do it. Since things get messy and you've created this bottleneck, you have to call out a special time for grooming. (This means that the ultimate goal of a formal grooming meeting is teaching the team how to groom without having a formal grooming session. It's not that hard. You've figured it out by reading a book. When everybody can constantly help keep things clean and organized as you move along, folks will be much happier and productive. As my mom used to say, instead of waiting until there's one big cleanup job, clean just a little bit as you go along. Makes life much easier.)

### **Introduce new information**. 

Sally is a Customer Service Representative in a mid-sized insurance company. She works in the same building as the rest of headquarters, just a few hundred feet away from the IT department.

Sally has found a bug in the software she uses everyday.

What does she do? Does she tell her supervisor? Fill out an online form? Just suffer and put up with it? Find another job?

These were the options she was given.

Sally entered the bug information. Two months later, when nothing was done, she entered the information again. Then again in six months. Finally she left for another job.

Joe is a Product Owner for a financial app that runs on three major platforms. His team works in a building 100 miles away. He has some new ideas for the app based on some conversations he had with UX experts this morning. 

What does he do? Does he wait two months until some kind of program-level meeting? Does he set up an online meeting? Nope. He was told that all he had to do was enter stuff into this magic tool and it would be done by the team. So he whenever he thinks of new stuff, he just enters it into the tool.

Now the tool has over 200 items that Joe and other people have put in. The team doesn't understand what the items mean, and Joe and the other business owners are dickering over which items go ahead or behind which other items. For many of the items, even the people who entered them can't remember what they mean.

Joe gave up on the tool. Now he calls the developer directly when he has changes, interrupting whatever was going on and massively changing direction of the project from day-to-day. Developers do not say nice things about Joe (They like him as a person, of course. He just drives them nuts as a Product Owner.)

Mary is a Senior Vice President at a manufacturing firm that's embedding software in their products.  When she wants something done across a complex system, she'll subtly ask several of the embedded teams to implement the feature, knowing if just one team delivers it, her goals will be met. Months later, during a sidebar conversation at a management meeting, managers figure out that several teams are doing the same thing -- and they're doing it different ways.

Louis is a supervisor in a regional office of a large government agency. Most of the software he deals with is outdated and brittle. Over the years he's seen a dozen different efforts to improve things. He's seen consultants come by with surveys, he's attended national conferences with other supervisors and sat on committees, he's been asked to write up his experiences in reports. There are four different systems for requesting upgrades, bug fixes, and enhancements. Working with none of them seem to ever produce positive results.

Louis has given up on change. Now he's just biding his time until retirement.

We understand the dialectic and Structured Analysis, so we know that all of these ways of adding information to a team are counter-productive. We also realize that there are people outside the team that have important information to add. The team has to have some way of interacting with outside folks using the dialectic to hone their shared mental model of the world.

You gotta add information. There are just a few simple rules that have to be followed to do it well. But they all have to be followed.

* Nobody but nobody adds information to a team's backlog aside from the team. People have to go through the team to make new information appear there 
* People who work physically near the team are the ones that can work with the team to add new information. If you aren't one of those people, you have to work through one of them. No "mailing it in" or using an online tool
* When you want to add information, you show up at a set time and have a conversation with everybody in the team. If you have formal grooming sessions, a good time for this is at the beginning of those sessions
* The team's job is to do the best it can to translate the universe you live in to the universe they live in. They may actually have to start modeling out your world, with Master Models and the rest of it, for it to make sense. (Remember, you should be able to do this quite quickly. Minutes, not hours.)
* At the end of adding information, the team should be able to walk you through your world, how you came across this new information and why it's needed. They should know enough of your world to be able to change their model so that it meets the needs of your model
* The conversation isn't over until the team can describe a test that everybody agrees on that would reflect the team understanding and correctly responding to the information you're providing
* There's no way that all of this can be guaranteed to be completed in a single conversation (although it happens that way most of the time for an ongoing, established product), so you have to be available for follow-up questions

For technology teams that use Scrum, the ideal situation for people with information to add is to wander down the hallway to their daily stand-up. Once that's over, raise your hand and tell them about what you'd like to talk about. At this point the team will self-scope and self-organize around the work instantly. Maybe they'll have to set up a meeting with experts and take a day to talk about it. Maybe you should just come down during the next grooming session. Maybe they're already doing that work and just need to tweak it a little bit to match what you're providing.

Maybe everybody just hangs out an extra five minutes and asks you a few questions. Boom. Grooming done.

By making the addition of work physical instead of electronic, you ratchet down the amount of churn that can happen while also reducing the waste associated with blindly entering things into systems where the items have to be worked and reworked, over and over again.

(Of course it can work without following these rules, and most of the time does -- eventually. This is what I've seen as being necessary to move very quickly and effortlessly to adapt to new situations.) The absolute best grooming I've ever heard of -- I didn't get to see it -- was an Agile Coach who went to work as a developer for a financial trading firm. They worked as solo developers, and they did financial trading alongside a trader. There was no wall at all between the work and automating the work.  Traders were expected to program and programmers were expected to trade. They worked in pairs. I believe this is about as optimal as technology development can get. That's nirvana.

### **Synchronize the Model**

If there is some kind of grunt work involved with backlog grooming, it's synchronizing the analysis model. It doesn't have to take long, but it has to be done regularly, religiously. It's like brushing your teeth. You do it and it doesn't feel like anything happens, but if you don't do it, all kinds of unpleasantness is on your way.

Behavior always seems to be the best way into scanning the entire Analysis Model.[^19-5] Go down the behaviors. Are we able to point to domain objects and talk about how they work together to make this behavior happen? For each behavior, are we able to point at the applicable supplementals and describe how they affect this behavior? Not using the model itself -- that's cheating. Can we do it just by chatting with one another? The real model exists in our heads, after all, and no matter what's in the EasyAM system, if it's not in our heads it doesn't exist.

[^19-5]: If I get bored, I'll start with the Domain Model. Or the Supplementals. It's all the same thing, anyway. People just seem to relate more to behavior, and if doesn't relate to the behavior list, it's out of scope. So if you want to start somewhere else, it's a fun thing to do, just always be sure you're not accidentally increasing scope without realizing it.

If that goes smoothly, go through each behavior and ask about actors. Who is the person/entity that initiates this behavior? Do they initiate other behaviors? Then triggers. What kicks off this behavior? Does it kick off other behavior? Finally outcomes. Do we know all the possible ways this behavior can end? Do these outcomes kick off yet more behaviors?

Scope yourself to a certain amount of time and quit when the time is up. If you've done the first couple of items above without finding anything new, next time start at the third item, then the fourth, and so on. In many ways this is like painting a landscape. First you sketch out the general look, then you pay a little attention here, then you pay a little attention there. Each time you look at your landscape painting your goals is sketch out a few more details. (Not go on a death march.)

You're not doing this to build a spec. You're doing this to do a cross-check between model items to see if there are important conversation areas you might have missed. Here's a hint: there always are. Once the model gets sketched out past a hour or two, it starts suggesting conversation areas and reminding you of things you that you probably wouldn't have thought of before. That's the magic.

### **Clean up the backlog**

Once your model is sketched out a little more and cross-checked, it's time to make sure your backlog isn't whack.

Most backlogs are whack. They're whack because the model keeps changing while the backlog doesn't (until grooming, that is.)

I'm just going to get the shocking thing out right away. You may want to get a grip on your chair.

***Your product backlog should never have more than 20-40 items in it.***

But Daniel, how can that be? We have a big project! A complicated system we're building! Funding for the next two years! How could that kind of work be covered in 20-40 items?

There are five and only five kinds of things that go in your backlog.

* Goals/Tests you are currently working on 
* Goals/Tests that you will be working on next 
* Goals/Tests that you need to start seriously thinking about (the next in line)
* Master Backlog Items 

That's it. Since your Master Backlog is a small list of things, 20-30 items, and since what you're currently working on doesn't really count here, all we're talking about is Master Backlog plus next up plus things to start worrying about. Assuming the max of 40 items in your MBL, and assuming you could work on a quarter of those at a time (optimistically), worst-case we're talking about 40+10+10. Sixty items. Most of the time it's around 40 or so. 

PUT BACKLOG GRAPHIC HERE 


### Verifies that we're ready to create executable tests for upcoming pieces of work

Everything that goes in our Behavior bucket describes a test, it's just more or less detailed. Associating that behavior with supplementals completes the description -- once the flow of the behavior and the detail of the supplementals are worked out. In fact, all of grooming, and all of Structured Analysis, is about continuing to develop the behavior and supplemental buckets so that we can take various intersections of the two to make executable tests. Describing and writing those tests, having them pass in the target system, those are the goals.

Soon, however, the moment of truth happens: we have to execute the tests. We run the test, it fails. We do some work, then we run the test again. It passes. We have completed that backlog item. That is, we have changed the target system such that it implements the behavior described in the test. (Remember, the target system doesn't have to be a computer system at all. It could be a set of corporate policies to help employee welfare, or a description of a fantasy world that our new novel will be set in.)

So the overall pattern is that we join up supplementals and behaviors to create testable chunks of future system behavior. This creates a testable chunk of work for us to do -- to make the test pass. Once the test passes we do this again. We continue doing this until the target system reaches a state we find acceptable.

What that executable test looks like depends on which layer we want to work in. 

If we're working in the Business Abstract layer (The Master Model), then the test consists of a verbal walkthrough with agreement. Validating and improving the Master Model through verbal walkthroughs is the heart of backlog grooming. A key part of this test is being able to describe various Business Realized goals that could all fulfill this test.[^19-7]

[^19-7]: So you're actually doing TDA as soon as you start double-checking your master model in the first conversation with the customer. Being able to describe a behavior using domain model words and listing the appropriate supplementals where everybody agrees and there are no open questions or things to add is the test. You'll make several runs at this until you get the test to pass. (This is why you don't want to fill out a bunch of detail until you absolutely have to! You'll never get a test passing.) Then more detail will come into the model as you continue to work it. The next time you make a run at it, the test fails. More work is needed.

If we're working at the Business Realized layer, then the test would consist of implementing or observing a physical business process and making sure that there aren't items from any of the buckets that you've missed. A key part of this test is being able to describe various generic computer solutions that could fulfill this test.

If we're working at the System Abstract level, an executable test consists of providing pseudo-code for how a computer program would meet the System Abstract goals. A key part of this test is being able to write actual code that fulfills this test. (Not necessarily writing it.)

In technology development, stories that we're almost ready to work on have to be developed enough to work at the System Abstract level. Most product/project backlogs consist of children of the Master Model at either the Business Realized or System Abstract level (or a mix of both. Nobody says you have to work in only one level.)

Of course, ideally you make a few lists to create a Master Model, talk about what kinds of System Abstract tests need to pass for a goal to be reached, then dive down into the System Realized level to make it happen. It's only when things simply must be more complicated that we care about knowing which level we're on.

TDA means constantly walking through behaviors, supplementals, and domain items at any one level to see whether is agreement that enough detail has been provided to make a test at one of the lower levels. (Not necessarily the next one down.) Analysis only exists to create tests that everybody agrees to, and it's constantly driving towards defining those tests in good-enough detail. Tests Drive Analysis.

## User Stories and Story Splitting

A lot of Agile folks call these backlog goal/test items "User Stories", They have a bunch of other terms too, like "Feature", "Epic", "Technical User Story". A few others. And then they use the terms to mean different things depending on which book you've read. I'm calling everything in your backlog a "User Story" because life is complicated enough as it is. A User Story is a testable chunk of work which describes future behavior in a target system. It's a match between Behavior and Supplementals which insists on a structure being created in order for the test to pass.

"But my User Story is too big for this next chunk of work!" is the most common thing I hear from teams that are new to backlogs and backlog grooming. "How could I ever make it smaller?"

The trick here is that once you understand what User Stories are, the intersection of Behavior and Supplementals, you can easily break them out into smaller pieces based on the details of the items in each of those buckets that apply to this user story.

Many times the first time you split a story is the first time you figure out a lot of supplementals that were hidden until that point. You just never think of them.

Let's say you are writing a complicated web page that does one Behavior. There doesn't have to be a one-to-one correspondence between behaviors and web pages but for this example let's assume there is. It was tough understanding this behavior, so you sketched out an Activity Diagram to describe the flow, which has one entrance point and six outcomes. 

Great Scott! You can't implement this complicated flow all at once! That's crazy! And it's the first story too! Heck it might take a month just getting the environment in place.

Okay so you're off-the-rails already. You don't "get the environment in place", you develop the environment a little bit at a time as you deliver goals, just like you develop the rest of the structural items. It all depends on which goals you are delivering.

*This means that environmental/build/deploy items should appear on your supplemental list*

If I'm delivering the "foo" goal, what kinds of supplementals might I need related to the environment?

* Show something to the user related to the goal
* Do something when the user acts (UX)
* Do something and update the rest of the system when the user acts (delivery pipeline)
* Show the right thing to the user 
* Show the right thing to the user when the user acts (ZOMBIES)
* (Rest of supplementals go here)
* Tweak the machine, ie. add performance supplementals as the system continues to mature

You've got six outcomes for your behavior. That's six different flows. For each flow, you've got these seven supplementals, plus whatever other ones your system has. If you wanted to have a status report that looked good, you could blow this out immediately into 6 times 7, or 42 small User Stories. 

For user stories that you're worried about doing all at one time, blow them out like this. I wouldn't add them to your backlog because you don't have anything to do with them accept decide to deliver them and then deliver them. (For a lot of people, this happens during a process called "Sprint Planning"). It's the last possible step before actually working on the dang things. They don't need to be in your queue because there's nothing for them to do there.

Instead, when it comes time to figure out what you can do, pull the little ones off and write tests, watch them fail, then change the structure and watch them pass. Many of these delivery supplementals will have tests that consist of functions that are reused over and over again. If you write a separate test for each story that has the only acceptance criteria of "show something to the user", I will come to your office and use invective and strong language until I hurt your feelings. Instead just write a platform tests that makes sure the pages are up, then add your page to the list when you come to that story.

You've split a User Story into 73 small User Stories. Do you have to keep all of those around on the backlog?

Heck no! If you're doing 12 of them and saving the other 61 for some future date, they don't go in the backlog. They don't go anywhere, since they are not tests that you currently plan to work on. I don't want to see them on your backlog. I don't want to see them on the wall. I don't want to see them anywhere. If you insist, stick them in the notes section of the appropriate Master Backlog Item. They'll be there for your consideration the next time you look at that item. Not before. Keep It Simple, Silly.

### **Tease out the best way the entire model might be delivered (Points, Estimation, and Other Games**

Finally we come to estimation, a subject that has caused much wailing and gnashing of teeth for some in the technology community. It seems that some folks have bosses that are assholes, and to prevent them from being an asshole, people want to remove estimation from the list of things a team might do. Replace it with the word "forecast". 

This is like preventing fires by outlawing the word fire and instead calling all fires "balloons".

Estimation can be important, and grooming is a good time to do it. But it's not important for the reasons you might think.

Let me describe a popular system for estimation that some folks use.

Take the entire backlog. Pick the simplest item. Call it a 1. For other items, **guess** how difficult they are to deliver compared to this one. Twice as much? It's a 2. Four times as much? It's a four. Total up the points. It's a simple game you should be able to play in a few minutes. The advanced version includes only using numbers that are doubles of one another (1,2,4,8,16...) or those in the Fibonacci or Lucas series. I like using the Fibonacci series because I like saying "Fibonacci".

Then, at some later time or date, take the "story points" for what you completed in one timebox and see how they relate to the total. Did you complete 10 points in the last week and your remaining total is 100 points? Then you've effectively "guessed" that you have ten more weeks to go.

This is easy, even somewhat frivolous and silly. When I first saw it, I was a bit astounded. Just putting numbers on things and adding them up could give you an estimate? Really?

Something weird happened. I saw it working, over and over again. But I don't think people understood why it worked. As long as the team was regularly playing this point and estimation game, looking at the entire backlog, after several rounds the estimates got strangely accurate.

Then I saw all the ways this was being done wrong. It was painful. I understand why many people refuse to do any estimating at all.

I saw people insist that these points had to map to some time period, like an hour or a day. This is a terrible fail. You might as well just estimate hours or days. The abstraction gets you nothing if you're just talking about time.

I saw people do the estimation at the same time they did points. This is also a terrible fail. The entire point (ouch!) here is to separate the guess about how complicated it is to deliver stuff from the actual projection of when things will be done. They're separate events. The projection doesn't even need the team in the room. It's simple math. If you put it all together at the same time, people are going to look at points as days or hours again. You're just doing some kind of weird kabuki dance in the middle of it.

I saw people take how much time they had for a project, then divide the number of time chunks they had, arriving at some weird number. Do we have ten sprints and 100 points in our backlog? Then we have to do ten points per sprint, dang it! This is a triple fail. First, it completely forgets the concept that the points for items will change over time. Second, it ignores any new items being added, and new items are always added. Finally it uses time to drive work. The work is the work. At the risk of being crude, if you change what the work is based on time (instead of what the users want), you don't know what you're doing. (Although it's perfectly acceptable to talk with users about what they actually want, of course. You just can't put the cart in front of the horse)

I saw people leaving the points from last time on the story for the next time the game was played. Well heck, if you're going to do that, people aren't really guessing again, are they? They're just looking at what the old number was and asking if anything changed. That might be an interesting thing to do, but it's a different thing from the way the game is played.

I saw people taking the points from one time period and then using that number to determine the next time period. Did ten points last time? Pick ten points of stuff for next time and do that. After all you did ten points last time, right? The failure here is that points are a lagging indicator, not a leading one. That is, you do what you can do. Points got nothing to do with it. Until you do it, you really don't know how hard it is to do or not. I've gotten to erasing points as soon as the game is finished to prevent this kind of nonsense. Do the points. Forget them. Do the work. Then offline, use the points to guess how much work is left. 

I totally understand why people don't like estimation. Points are a simple system but hell if we don't screw it up a lot.

The point game does this: the entire team walks through the entire backlog working through a mental model of how each item might be delivered. They do that over and over again, and as they get better at delivery and understanding the entire project, they get pretty good at guessing how relatively difficult things might be.

At least that the way it reads in the book.

But something else happens that we know that the book writers didn't: as the team walks through an imaginary delivery of all these goals, they're creating a shared Meta model of execution which gets more and more accurate with practice. 

We're back to alignment and shared mental models again, only this time in the **Meta** genre, not Business or System. What we're doing as we deliver things and think about how we're going to deliver more things is come together on a system for how we deliver stuff. That's the real value of the point game, which has nothing to do with estimation. It creates a shared Meta Abstract To-Be model.

In the deck example, we did the same kind of thing. As we continued playing with our models, bouncing them up against behavior and supplemental items, we were also thinking about how we'd build the deck.

There's also an aspect of this that's more social psychology than anything else. As the team keeps estimating, making stuff, then estimating some more, they end convincing themselves that whatever their model is, that's the true reality. And it become reality for them simply by them all agreeing on it.

It's like placebos. It may be total crap *how* it works, but it actually works anyway, so who cares?

If you like estimating, then estimate, using whatever method works for you. But whatever you do, you need to engage the team mentally on a regular basis with thinking about the entire model and how it will be delivered, not just what items are in the formal, written model and how they connect.

This book is not about Agile, Scrum, Story Points, or sprints. It's about what's going on behind-the-scenes in the minds of people who create new realities for folks. A hundred years from now maybe nobody does Story Point estimation anymore. They'll still need to be going through the entire backlog creating a shared mental model of items in the Meta genre.

Now let's dig in to see grooming in action using EasyAM.

