## Chapter 15
![Your new business awaits!](images/deck-design-from-wiki.png)

After trying your hand at dog houses, dental franchises, Mars colonies, and several other jobs, you've decided that the best time you had was back when you were building stuff. You've also decided that dog houses suck. What to do? Build backyard decks, that's what!

After reading this book, you're determined to do this the right way, maybe even do a little too much up-front work just to make sure you do a good job. When your first customer comes along, instead of just chatting and sketching something on a napkin, you chat and jot down your master model as you go.

What does the world of backyard decks look like in this guy's mind? After 30 minutes of chatting, here's your Master Model sketch.

**MASTER BACKLOG**

- cookout food
- nap in the summertime
- entertain friends
- soak in hot water in the winter
- sunbathe with my friends

**MASTER SUPPLEMENTAL MODEL**

- Has to meet local building codes 
- Has to be easy-to-use
- Has to look nice to the neighbors 

**MASTER DOMAIN MODEL**

- food
- hammock
- hot tub
- recliner
- table 
- chairs 
- gas grill
- family 
- friends 
- hobbies

Also, there were a few times where he started giving out structural pieces, like he was designing it in his head.

- "Those steps will need to be six-feet wide"
- "The railing should only be a couple of inches apart."
- "Boards ought to be made of that red stuff you see in pictures"
- "I don't want to stub my foot on a nail"

If hadn't read this book, or if you were like many technology teams, you'd take these statements as requirements. "Oh, we will have steps that will be 6' wide. Here are specs on the railing. And wow, looks like we'll be buying redwood! This will get expensive! Also we should buy headless nails. Do they make those?"

But nope, you ain't falling for that one. ***All structure is deriviative.*** That means that whenever a customer or Product Owner starts talking structure, it's the result of some kind processing they've already done in their head. Maybe what they concluded makes sense. Maybe they had bad or incomplete information. Maybe they're thinking about a problem from a different angle than you are. (This is actually the most likely thing to happen. If you're talking to a guy about building a backyard deck, he's probably loading up a mental model he shares with the family about outside fun at home. That's got all kind of items and linkages that you don't know and probably don't matter)

If you take structural information at face value, you've abandoned the dialectic. That's not happening.

So you push back, gently. You list those sentences and say you'd like to talk about them further. After just a few minutes, you've eliminated this extraneous structure stuff and gained more insight (and continue to align mental models with your customer)

Here's how those statement decomposed:

- "Those steps will need to be six-feet wide" -> Uncle Joe and his wife Edna are very large people who like to hold hands a lot. The steps need to accomodate them without making them uncomfortable
- "The railing should only be a couple of inches apart." -> He read somewhere that babies can get their heads stuck in railing and die. You point out that building codes cover this problem and a lot more. Is it okay just to abide by the codes, instead actually having a 2" gap? Or is there something else? Nope. So this item is deleted
- "Boards ought to be made of that red stuff you see in pictures" -> He wants redwood *stain*, not expensive hardwood. He doesn't know what he's talking about, he's never built a deck. He likes the redwood stain and wants weather protection for ten years
- "I don't want to stub my foot on a nail" -> He visited a friend last year who had an old deck and stubbed his foot on a nail.

Out of all of that, we've got three supplementals. One Business Abstract Supplemental: "All entrances must comfortably accomodate two large people side-by-side". We've got two System Abstract Supplementals: "Structure must be impervious to weather for ten years", and "Use joining technology that doesn't poke out after wear (screws, for example)"

We have no structure information, although if we had let him, he'd probably start sketching out deck designs on a napkin. Then he would be doing the work, we'd just be preparing materials and joining them. There are a ton of technology teams that think this is an ideal situation. I feel sorry for the people who pay them. 

We've also began to establish some rapport with our customer, learn about his life. Maybe we've started to become friends. Remember, he doesn't know Structured Analysis. From his side, we've taken care to learn more about what's important to him. This isn't you taking over the project. This is you showing that you're actually concerned about what the guy wants and the quality of the work.

We've asked permission to learn about what he really wants and what he's afraid of, and we've asked him if we could have the honor of sketching out some ideas and talking to him about them instead of having him giving us a model made out of Legos or something. All of this adds what we know to what he wants.

So we have three more supplementals. For now we'll put the System Supplementals up at the top of the model, in the Business Abstract spot. Easier to use that way. Sue me. We've also got a new behavior, one that seems obvious but was never brought up: I need to enter and leave the deck.

### Loading up EasyAM 

So that's our Master Model. We ask our customer out to lunch and while we're waiting on the hot dogs, we enter the Master Model into EasyAM. We make a text file named "2018-05-01 dbm Initial Notes.amin" The contents look like this:

![](images/chapter15-easyam-1.png)

