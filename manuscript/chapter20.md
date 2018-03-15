# Chapter 20

Congratulations! You've just received a large grant from a well-known charity to write software to support oppossum flying schools. Flying squirrels get all the good press, and the group "Opossums United Curicculum Help (OUCH!)" wants a computer program to help those brave folk around the world who are teaching opossums to fly. They are too often forgotten. Have you ever seen a fundraiser for oppossum trainers? See?

Along with the grant came a first-class ticket to Hooterville, Illinois, home of the World Famous Peter Principal's Precision Possum Pilots, school for possums wanting to break free of the usual midnight snack around the cat bowl and launch themselves into the void.

As you walk through the gates and onto hallowed ground, a plaque welcomes you.

![](images/opossum-mypossum.png)

When you meet Peter, owner of the school, the first thing you ask him is if you and he can just work side-by-side for a few weeks. You'll help him with the possum pilot preparations, he can help you with the coding. This would create an instant feedback loop, eliminate any kind of analysis or backlog, and cut the crap down to the minimum-needed to get this software written.

This does not work for him. The demands of opossum organizations are such that we'll have to set up some kind of schedule. In addition, there are other possum schools that have to be happy with the software, so Peter isn't a customer. He's just a guy to help you understand the needs of possum people.

-sigh-

Ok. So who *is* the customer? You look up the number to the OUCH! people and give them a call.

As it turns out, they don't even want software right now. All they want is you to come back in a month or two and pitch them on what software *might* look like.

You've read this book, so you know that work without a test is breaking the rules. How are you supposed to know that the model is developed enough without a test? You could stop after five minutes. You could take five years. This is the crux of the problem with analysis paralysis. No tests, no end.

How about if you built a *prototype* application while talking to Peter? It'll take the same amount of time either way, and you'd feel much better to have something to show them.

They're okay with that. So you have two goals in mind for your work:

1. Understand the world of opossum pilot training enough to propose and explain a software app, and 
2. Build out a real app to validate any unusual or tricky aspects of helping these possum people out 

You spend an hour with Peter and come up with this Master Model.







## Grooming Examples With EasyAM

Pointing
Splitting
Bug dump
Feature request


1. You are not allowed to have any important conversations unless it's to validate items already in the analysis (shared mental) model
2. You are not allowed to add things to the model unless it answers a relevant question or fixes a failing test at the current level 
3. You stop adding things to the model as soon as there is agreement that enough has been described to create a failing important test at some lower level

The ordering of tests by importance is called the backlog queue


