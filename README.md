# Career-Track---Readings

## Quantity Trumps Quality
I think was this reading is ultimately trying to convey is that sometimes when we're so focused on making the perfect things, we waste an inordinate amount of time trying to nail down what that is before ever actually doing anything. Paralysis by analysis if you will. The other takeaway for me from this reading is that quality, with most skills/crafts, comes with repetition. Repetition in this case demonstrated by quantity.

## Clean Code - Chapter 1
Messy code makes everything take longer. In the beginning it's typically accepted as okay to meet deadlines etc. but rarely is this the actual case. In fact often times deadlines are still not met and once the code quality starts getting sacrificed for finishing it only gets worse. As code gets more and more messy it takes longer and longer to do things that should have only taken a few hours. This is very much a snowball effect.
Clean written code accomplishes one thing really well. It's simple and reads like well written prose. It should be clear in it's decision making, easily enhanced by others, and tested. Clean code appears to have been written by someone who cares. When it is read by others it should be obvious and absolutely what was expected with nothing extra, espeically duplications.
Keep in mind that code is read 10 times more often than it is written. This is important because if you're trying to enchance existing code and you can't even read it how can you possible make it better? It's not enough to only focus on this in the beginning, but also important to keep the code clean over time. Leave code cleaner than when you arrived.

## Red, Green, Refactor
Using these steps we can begin implementing Test Driven Development in our coding practice:
Red - what do you want to develop
Green - how do you make your tests pass
Refactor - how do you improve your existing implementation
In the Red we need to identify what we want our code to do, ideally 1 thing that can be stated in 1 sentence. We develope a test that will test our code to see if it does this one thing consistently. When we run the test it's going to return an error because we haven't written any actual code yet.
In the Green we have our test that is failing and we need to write code to make it pass. We don't worry about efficiency or speed or anything like that, but we simply focus on writing code that our passes our tests.
Now that we have passing tests we can begin to put more thought into our actual code so that's more simple and more efficient.

## The Cycles of TDD
Customers value two things about software. The way it makes a machine behave; and the ease with which it can be changed. Compromise either of those two values and the software will diminish in real value to the customer.
Refactoring is not something you do at the end of a project; it's something you do on a minute-by-minute basis.

Nano-cycle
3 laws of TDD that you follow on a second-by-second basis:
1. write a failing test before any code
2. do not write more of a test than is sufficient to fail
3. do not write more code that is sufficient to make the test pass

Micro-cycle
This cycle is on the minute-by-minute scale and happens every dozen or so cycles of the nano-cycle.
1. create a failing test
2. write code that makes the test pass
3. clean up the code to make more efficient and simple

Milli-cycle
This cycle occurs every few minutes. As our test suite grows it can become very specific, to combat this we need to make code more general. "Programmers make specific cases work by writing code that makes the general case work." If code changes we make so that a test will pass creates problems passing other test than our code has become too specific and we need to back up and start again.

Primary-cycle
This is hour-by-hour. Every hour or so we need to stop and make sure that we're not encroaching on any significant architectural boundaries. Where are our boundaries, or where do we need to put some to constrain our project so that it's still heading toward the ultimate end-goal?
