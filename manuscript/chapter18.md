# Chapter 18

![The Test-Driven Analysis Constellation (Subject to revision in later editions of this book)](images/Test-Driven-Analysis-Constellation.png)

## Backlogs

Most people keep a list of to-do items with them during the day. For many, there's nothing like the happiness of checking another item off. There are hundreds or thousands of books that all encourage people to make long-term goals, then short-term goals, then to-do lists. It's like a pyramid! You can master the universe through this method of goal/task breakdown.

People really love this stuff.

I am not one of those people.

On a personal level, I believe that mission translates to values + habits and that leads to success. That is, you get further by creating habits and a lifestyle that reflect your values and advances your mission than you do by trying to complete some kind of top-down masterplan of where you want to be in five years. You have no idea what things are going to be like in five years, and you have no concept of what things might be feasible or impossible.[^18-2]

[^18-2]: Scott Adams covers this in-depth in his "Goals are for losers" essay. [http://blog.dilbert.com/2014/01/21/goals-are-for-losers-passion-is-bull/](http://blog.dilbert.com/2014/01/21/goals-are-for-losers-passion-is-bull/)

Of course, that kind of top-down planning might make sense in a fixed domain where the number of unknowns is drastically reduced, like sales, but not in an environment where everything is poorly defined and changing. If you're in a factory building widgets, you know how widgets are put together and what widgets look like *before you start anything*. That means everything is defined. In that case, certainly big physical things break into little things.

But if you're building a new type of battleship that's never been built before, you have no idea what it's going to look like or how you're going to put it together -- until it's all done. There's nothing defined. (Except maybe a lot of baggage people might bring into the discussion when the term "battleship" is mentioned, some of which might be terribly counter-productive) If you start breaking down something that's not defined? You end up defining it! So what's the purpose of Analysis, then? You already know there's going to be a gunwale. Look, there on page seven it says "build gunwale". You've short-circuited the most important part of the work simply in a desire to have a big list of things and all of your questions answered.

I think this is why you see so much of this break-your-goals-into-tasks kind of advice from people who have built their own world to live inside. Once you construct a machine to live in, such as car sales, you can take a much more structuralist view of life and success. You know what all the pieces are. You built them. That kind of thing makes sense. (Startup guys call this "building the flywheel". We'll go over startups and flywheels in the last section.)

When we think top-down is we bring a bunch of baggage along with us, intentionally or not. Since there are a ton of unknowns about planning how something we've never done breaks down into tasks, and since there are even more unknowns about doing things we've never done before --- we make stuff up.

That's a feature, not a bug. Humans are able to exist as a sentient species on this planet because we are able to take vague, fuzzy, incomplete data  --- and construct a narrative and a universe around it. Get bitten by a clown when you're a kid and you avoid clowns for the rest of your life. That may be a horrible stereotype to have, but it prevents you from future clown bites. Our ability to imagine narratives and stereotype is a survival skill.

There's a difference between goals and tasks, and it turns out that understanding that difference helps with backlogs and grooming.

**Goals** are things in the future you want to accomplish but don't know how. Goals are a combination of Behavior and Supplemental Abstract To-Be items. They can be either **Business** or **System**. "I want to run the five-minute mile" is a System goal. (Your body is a physical thing). We are describing a future System behavior, running the mile. The Supplemental is the 5-minute qualification. "I want to reduce claims processing time by 30%" is a business goal. Claims processing is an abstract business process, at least at the level we're talking about it now. There are a ton of physical system linkages in there somewhere that we would need to discover.

Goals have tests. Without an executable test, we don't have a goal. If I go out running, you can take a stop-watch and see how fast my mile is. We can dig out records and find the speed of claims processing. No test, no goal.

**Tasks** are Meta Realized Behavior, that is, they're things that you (or your team) go out and do. *Tasks have no relationship to goals except in our own minds* They are independent, stand-alone units describing *activity*, not *value*. We think of a goal, then we *imagine* the type and number of tasks it takes to reach that goal, then we start doing them.

It's important to understand that there is no relationship between tasks and value. In the movie "Christmas Vacation", one character praises another character by saying "he works hard", to which the reply is "dishwashers work hard". Activity and value are separate things.

Since goals are another word for tests and tasks are supposed to be in support of goals, it stands to reason then that the more tasks you do before executing a test, the more likely you are to be wasting your time. Ideally you never want to get more than a few hours between executable tests. A few minutes would be optimal. And this is easy enough to do. (Trust me on this)

In our deck example, as soon as we had our initial conversation and gathered some behavior and supplementals, we created something structural, the diagram of the deck. Then we tested our behavior and supplemental notes by working with the derived structure to see if it made sense to us.

The structure does not have to be part of some assembled finished product, but it must be structural. That's the only way to test behavior and supplementals, by looking at the derived structure.

So while we had a few tasks to get things organized, maybe print some stuff out, gather some modeling tools together and so forth, we were immediately back into testing mode.

Good **Backlogs** are a list of future behaviors the target system needs to exhibt. They're all Behavior To-Be items, whether at the Business or System level. Some backlogs are full of to-do items. We call this "Tasking out the backlog", and it means that instead of talking about what the system will do, we're talking about what we're going to do.

This is an excellent way to make really good status reports without accomplishing anything of value. 

I've seen a lot of poorly performing teams and organizations, and almost without exception I see tasking out the backlog as a key component of poor performance. On dozens of occasions, sadly, I have walked into programs where there a bunch of teams slugging away at something. Performance was down, staffing costs high, stress levels unacceptable. In every one of these cases, when I look at the team backlogs, they are full of tasks, not testable goals. (Behavior to-be matched up with supplementals)

Somebody, somewhere, at some time made some kind of mapping between goals and tasks -- but that person is not around anymore. The team and developers can sort of tell you the purpose, but there's no feedback loop. At the end of the day, they're just checking off boxes on a to-do list. 

Watching teams struggle like this, over and over, watching marriages crumble, people have heart attacks, and companies fail? That's the reason I wrote this book.

## Your Model of how Work Happens is all Wrong

It's one thing to talk about how tasking out the backlog is wrong, and how we want to reduce the "suspense" time between tasking and testing to just minutes. It's another thing to deeply realize what an anti-pattern this is.

Humans think naturally in terms of structure. Our minds are constantly combining behavior and supplemental information to create structural models that we accept as reality.

So when we approach a new problem, we approach it as a structural matter, which works in 99% of all situations. Need a chair? Make these structural pieces and put them together like so. Voila, a chair. This is the way nature works.

When we became industrialized, we started creating things using assembly lines and stations. Station A made these structural changes. Station B made these changes. We combine the various sub-assemblies into the finished product. In short, to build something, we break it down into small pieces, build each piece, then put the pieces together.

Beginning formally with a guy named Frederick Winslow Taylor, but informally a long time before that, people decided that to build stuff, you had to create categories and manage those little categories. Managers did management-kinda jobs. Head riveters riveted heads. A modern factory is a wondrous example of taking something complex, breaking it up into small pieces, then optimizing each piece.

The problem is that this way of doing things only works for physical things, not creative things. When we built the deck, the analysis work we did was the creative part, coming into alignment with the customer, trying out various physical models in miniature form, and so forth. The actual building of the deck was mechanical and rote.

Anybody with expert knowledge in carpentry could build a deck given the plans. We could create a factory for decks where robots do all the work and 50 decks are made in an hour. But this isn't what we mean when we tell people we built a deck for somebody. At least it isn't if we're a good worker.

Modern management theory is all about optimizing the machine. A business is a machine that makes money, just like a factory. We optimize how each of the workstations perform and we end up optimizing the entire thing. To manage a business is to assume that there already is a machine in place that needs tweaking and ramping up.

Managers are about codifying work into rules that control and implement flow and then optimizing the rules and the flow. Their job is to replace you with robots. There's nothing wrong with that. Nobody wants to be working in an 1880s sweatshop anymore. But the type of work that this represents is not the type of work Analysis covers. This kind of work assumes all the questions have been answered and there is no shared mental model to create or maintain (Insert long discussion here about how in many ways they may be wrong, but that's for another day.)

There is another business process which is, in some ways, the antithesis of modern management. It's called value discovery. Value discovery is what we've been doing with Structured Analysis; orienting ourselves in somebody else's world and coming up with stuff they would like. A successful startup combines value discovery into a machine that then can be managed. (Here is also an explanation for why so many great startup founders need to bring in professional management just when things start to take off. Management and value discovery are different skills.)

What this means is that if you're interested in doing Structured Analysis and/or value discovery, 99% of the books out there are not for you. In fact, they will lead you down the wrong road entirely. If you've been a great programmer, or have a sharp, analytical mind, the way you see and decompose problems is exactly the opposite of what's required in Structured Analysis.

I can almost guarantee you that whatever your background, it hasn't prepared you to break down goals into tasks in a way that actually works over time.[^18-4] In startup work and general analysis work, what we find is that we continue to apply things that worked for us in the past to the current situation, because humans. And then we waste a lot of time and money.

No matter how smart you are, your instincts will lead you wrong. Every time.

[^18-4]: Improv comedy might be a background that would be helpful. I am not sure. I have friends who are experimenting with teaching teams by way of improvisational comedy lessons. I have no idea how successful it is, but I would like to observe it a few times.

## But I Know My Backlog Item Isn't Behavior

There are a few common scenarios when folks think they know for sure that their backlog item just *can't* be behavior.

*The customer told me he needed a red button.* If the guy directly tells you he wants to see X, then that's a backlog item, right?

Wrong.

As we learned in the deck example, whenever you take these things at face value, you cheat both the customer and yourself. In that example, the customer just *knew* the deck steps had to be ten feet wide. But what he really knew was that he had a couple of common visitors that were rather large, and he didn't want to do anything to make them uncomfortable. That supplemental, not the structural size of the deck, was important to a lot more than simply the stairs.

Whatever the structure, ask yourself what behavior and supplementals it satisfies. Then ask where those pieces apply in across the rest of the analysis model. Most of the time when you get a structure request, it's because the customer has been doing analysis for you in their head, "helping" you. After a couple of times walking through how you tease apart these requests, they'll be more than happy to work with you on the rest of them.

*We're doing data warehouse work.* Data warehouse work is a bit of an odd duck because many times it looks like software development when it's not. The key term is "warehouse". You're not building a warehouse. The warehouse already exists. You're just putting stuff in and taking it out.

In many cases you're providing views into existing data as part of a larger effort. In that case, the larger effort should manage the analysis. All you have is tasks to make their tests pass.

In other cases your job is to move hunks of data around, bits of structure. The natural tendency is to organize your work around the structure. Instead, organize your work around automating the move. Your job is not to move these 17 tables from one place to another. Your job is to write code to move those 17 tables. Same result, different way of looking at things.

*We're working on an architectural tier*. We saw this a lot in the latter part of the 20th century and the beginning of the 21st, but it's slowly dying off, thank goodness. The concept went something like this: because we are deploying our system in layers, and each person/team is responsible for a different layer, our work is to put together and maintain pieces on the layer we are responsible for.

It is not. You have organized your work poorly. Start over. 

Here's the reason why. In technology, there are infinite ways to group and organize your solution. This is a bug, not a feature, because *organizing your solution and organizing your work are two separate things*. Yet people seem to keep conflating them.

There are 20-person teams, right now, who are struggling with writing a new log-in screen. Why? Because everybody in the room is an expert in one area. One person is an expert on security. Another on mainframe access. A third on UI. We have a UX person, a front-end person, a back-end person, a corporate policies person, a representative from the cloud group. It goes on and on and on. Every year new technology comes out, new specialties are created, and the team size grows.

Solving problems stops being about solving problems and starts being about making sure all the check-boxes are checked.

And each of those people? They each have been to several specialized training sessions where they were taught how to organize their work around their specialty. Those back-end guys are experts at creating projects to manage back-end work. The UX guys have an entire playbook around making good UX happen.

If you don't know what you are doing, if you lose track of the goal and instead focus on the people or technology, you'll end up pulling out each persons work pattern tasks and stuffing a backlog full of it. Then, when somebody tells you the backlog is for goals only, it doesn't make any sense. How can we get the database done if we don't have database things on the backlog?

But that's not the way it's supposed to work. What's supposed to happen is that you have a goal/test to meet, and then anybody involves adapts their work pattern to reach that goal. If they don't understand how to do that? Then we need to train them. They have been misled, probably by other trainers.

Over time, all of the jobs that are necessary get done, but they get done in increments as the target system begins to exhibit more and more new behaviors. Nothing goes away. All of that cool engineering you learned in school is still applicable. Every role or layer just isn't the center of its own little universe. You just need to look at things the right way, instead of the wrong way. Don't let your natural inclination to become an expert in one area get in the way of the team staying laser-focused on goals and tests.


## Test-Driven Analysis Redux

Test-Driven Analysis means we're always throwing behavior and supplementals together to create some structure for approval or disapproval, to pass or fail tests.

If our work is shaped around conversations, then we never have a conversation without a piece of structure and a test we bring and manipulate to get feedback on our behavior and supplementals. If our work is shaped around 2-week sprints, then we never begin a sprint without structure and a test we bring to define what done looks like. If our work is shaped around writing a computer function, then we never begin work without structure and a test we bring to define what that function's successful conclusion looks like. 

As they used to say when I went to school, it's turtles all the way down, folks. The only difference between conversations about Business Abstract stuff and System Realized is how the tests are created and executed.

Whatever level we're talking about, we have questions. We ask them. We get new information. We update our mental model (perhaps our written one as well, depends on the situation), then we create a test. We execute that test. We gain new information. Go back to the start and begin again.

And that takes us to Backlog Grooming.