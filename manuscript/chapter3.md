# Chapter 3

How would you communicate with aliens?

The usual answer from sci-fi and science is that we would use some sort of mathematical substrate. In Carl Sagan's book "Contact" humans receive a signal full of prime numbers. In "Close Encounters of the Third Kind" there's the math of music. SETI scientists have attempted to communicate by monitoring radio signals around the wavelength of hydrogen, which makes a ton of assumptions: comnmunication would be by radio, atomic wavelengths hold some sort of curious pull on species wanting to talk, and other species actually want to communicate, among others.

In the "Three Body Problem" the issue of communication is almost hand-waved away by author Liu Cixin, which is actually good, because most of the time this topic is done poorly.

There is one notable exception: the 2016 movie "Arrival". Lots of plot problems are solved by having the aliens arrive at Earth and hang out in giant eggs, waiting for us to try to communicate with them. In fact, the entire plot revolves around the question of how to communicate with aliens.

And it's not math. Instead you end up using some ideas kicked around by some guys named Sapir, Whorf, and Chomsky.

Sapir, Whorf, and Chomsky were linguists. These are folks who study languages. Linguistics is a relatively new science. The general study of languages, of course, has been going on forver. But studying how all the different languages are the same and different really started happening only in the last 150 years or so. 

There are a ton of interesting debates going on in linguistics, but the one that appears in the movie concerns the Sapir-Whorf hypothesis and linguistic structuralism, probably best-expressed in Chomsky's "Syntactic Structures"

Don't worry! There won't be a test.

All of this is really about one question: is language mostly determined by the culture we live in? Our world, our values, our feelings, and so forth? Or is language simply a formal construct with various pieces, like a building being made out of bricks.

On one hand, the SW guys felt that your life and values, the way you think, was tied hand-in-hand with the way you expressed things. The Intuit have a bunch of different words for snow and ice. We do not. That's because it's not part of our way of life.

On the other hand, the Chomsky/structural guys felt that language was simply a type of program that runs on human hardware. Chomsky was able to create a system where he could take any language and break it up into tiny pieces and rules. The brain was an operating system that used language in the way described by Chomsky. The actual language itself was just an app running on the operating system.

Let's say you were solving a problem, perhaps creating a new product for weasel farmers. The Sapir-Whorf school would advise you to become part of the weasel-farming world, live and breathe the life of a weasel farmer! Of course they would also tell you to understand the formal science needed to make the product. The Chomsky guys would tell you to gather as much information as possible about weasel farming, tagging the information and how it's structured into a formal system, a "language of the weasel farmer". Of course they would also tell you to understand the formal science needed to make the product. They might even suggest that there is a mapping between the information you learned and the product you're building.

If you've been around computer programming for any length of time, some of this should sound very familiar. The SW folks are the ones telling you how important it is to be as close as you can with the user of the product. Nothing can take the place of that! The structuralist folks are the ones telling you how programming is just a matter of mapping the language of the user into the language of the computer. Everything is about experiences, values, and cultures.

Anybody remember Model-Driven Development? The idea was that using the Unified Modeling Language, we could construct a model of how concepts existed in the mind of the people we were trying to help. Then? There was just this magical transform that happened that maps the symbols and structure from the user into the computer. Everything is about symbols, grammar, and mappings.

In the movie we see this happening almost as soon as the aliens arrive. The military wants to know: are they going to attack? What are their plans? Are they peaceful?

The linguist, played by Amy Adams, points out that these kinds of questions are the questions you can ask at the end of your investigations, once you have some idea of how to communicate, not at the beginning. It's not simply a matter of constructing some kind of alien language dictionary, where you look up one word in English and then substitute the alien one. We know nothing about their way of life. Even if we knew the alien phrase for "we come in peace", it might not mean to them what it means to us. Lots of folks throughout history have come in peace and ended up destroying the cultures they came into contact with.

There's always a tension between the people who need to get something done right now and the people who need to understand what the heck is going on before they'll do anything. Both sides have a good point. There's a similar tension between the Sapir-Whorf folks that tell us language is all about culture, the two are tied together and can never be separated, and the Chomsky folks that tell us language is simply a mechanistic contrivance our brains have evolved to communicate.

As we'll find out in this book, both sides are right. Both sides are also wrong. For now let's just look at how we solve the problem of getting started.

In the movie, the way they get started is by meeting face-to-face with the aliens, then pointing to stuff and making the sound that represents that thing. The linguist points to herself and gives her name. Based on history, this is the way people of different languages have always learned each other's language. They begin with proper nouns. No matter how you put together a language, there has to be some abstract symbols or sounds to represent physical objects.

We restrict the area of engagement as tightly as possible, making what could be an impossible problem much easier.

This is also how we're going to handle information flow, by restricting the area of conversations to the point that having good conversations becomes much easier.

We're going to add a tagging system to our information as it is created and consumed.

First let's clear up some terms. We have a bunch of words that kind of mean the same thing. There's the general term "conversations" that everybody likes. What makes a good product? Good engineering and good conversations! But I can have a good conversation about football. It's not clear what "good" means. There's the really good "dialectic" we just learned. A dialectic is what makes a good conversation!

I'm going to use "analysis". If you'd like a bunch of big words all at once, analysis is dialectical conversations around one particular domain. It's everything we do while talking about our work aside from actually doing the work itself.

If our job was digging holes, analysis would be dialectical conversations around which tools to use, how deep to dig the holes, why we're digging the holes, how many holes to dig, and so on. It's not the work of digging the hole itself, it's the critical conversations we have all around the work.

In "Arrival", analysis was all of the conversations aside from the aliens actually talking to the linguist. It was the planning, talk about how to do decontamination, the discussion of what topics were next, the coordination with the other groups, the lecturing on how to communicate with aliens. All of the conversations "around" actually talking to the aliens was analysis. Analysis sets the stage for doing the work.

So now we have a second big word that I expect you to use from here on out! Woo hoo! **Analysis** *Analysis is the use of the dialectic -- asking humble, pointed, direct, and honest questions back and forth among friends seeking a common understanding -- in order to solve a particular problem.*

Information flow optimization is providing the right amount of information at the right time to support effective analysis.

This book is like a lego set. We're starting out with little bricks. When we're done we'll have computer programs, languages, workflows, all kinds of cool stuff. But it all starts with these little bricks.

## Genres

The information we're managing supports analysis. And to make something really tough really easy, we limit that analysis to small pieces, or domains. Otherwise analysis would just be talking about anything at all tangetially related to what we're doing. We gotta limit stuff.

There are three domains (let's call them "genres") of things we talk about, no matter what we're doing. There is the genre of the problem we're trying to solve. There is the genre of how we're going to solve it.

That's it. If you wanted a simple three-way system of categories, you'd split along these lines: universe of the problem we're trying to solve, universe of the solution we're making, and universe of the way we work. Each of these is its own little special land with terms, phrases, jargon, ways of doing things, values, culture, and so on. Each genre is completely different. They are all foreign lands, and we should never expect languages and phrases that work in one land to work in the other -- even if everybody speaks the same Earth language. A "customer" in terms of the problem we're solving is a completely different thing from a "customer" in terms of how we run our business. And that's a completely different thing from some database table or class we call "customer"

Yes, the word is the same. No, it does not have the same meaning. 

In the movie, they took a strong Sapir-Whorf stance. Nothing could be accomplished until they started to learn the culture of the aliens, and once they learned the ways of the aliens, it actually changed the way our brains operated.

That's completely far-fetched for sci-fi, and no linguist I know about would take Sapir-Whorf that far, but you'd better believe it like a religion if you're moving information around to make things for people. Each of our genres is its own universe, and as we learn more and more about those universes, it will change the way we think about things.

Some of the worst business books I see are books that immerse the reader in one of these universes with the implied idea that by learning about that universe, the reader will better be able to do their jobs. This is only false, it hurts the readers. By focusing on one genre, say "how to write programs", the only thing we do is increase the density and complexity of the language around that genre, which can, oddly enough, make it more difficult for others to in another genre to be understood.

I see management books and classes that act as if you can be a manager (which is all about how we're going to solve things) without regard for the actual problem you're solving or what you're actually making. Management is supposed to exist as some sort of abstract world on its own. I see programming books and classes that act as if by somehow learning the tiny intricacies of a programming language you'll know anything about how to organize the overall work, or what kinds of lives the people you're trying to help live. 

Don't get me wrong. These things are extremely important. But they're only important as part of a big-picture view where you learn stuff to go do something useful in life. And to do that you have to learn stuff and operate in all three of these genres. It's like training people to be excellent taxi drivers by sending them to four years of learning about how cars work.

For brevity, let's call our three genres **Business**, **System**, and **Meta**. 

The Business genre is the universe of people we want to help. You may have heard of it being called the "Problem Domain" by some folks. It consists of language, rituals, values, and wisdom that has nothing to do with technology. It's just about people.

The System genre is the universe of the finished product, the thing we're doing. You may have heard of it being called the "Solution Domain" It consists of language, rituals, values, and wisdom that has nothing to do with people. It's just about making stuff, whether it's a computer program, a bridge, or an outline to a novel. It's just about the product.

The Meta genre is the universe of people making products, our system for doing our job. You may have heard of it being called "Process" It consists of language, rituals, values, and wisdom about our working life.

Let's recap where we are. Good information flow and management supports analysis (dialectics) around our job. To make these analysis conversations as easy, quick, and thorough as possible, we need to narrow our scope of engagement. Every conversation can't be about life, the universe, and everything. To narrow our analysis conversations, we've got a tagging system. Our first set of tags is called the genre tags. They are Business, System, and Meta.

There are only about a dozen tags we need to learn in three different sets. We'll go over them in the next chapters. Once we've learned our tagging system, then we'll move to application.

This process of having a fixed way of organizing information in order to make it more useful is called **Structured Analysis**. It's the reason for the first section. Once we understand Structured Analysis, you'll find that a bunch of things that used to be difficult suddenly become very easy.

