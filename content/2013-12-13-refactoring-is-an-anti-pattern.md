layout: post
Title: Refactoring is an anti-pattern
author: devcurmudgeon
date: 13/12/2013


I thought I'd written *more* than enough words on [refactoring](http://www.devcurmudgeon.com/2010/10/02/i-dont-like-your-code/) already, but maybe I was too cryptic. 

So here's my version 2.

Let's start by noting that most of the folks who claim that they are 'refactoring' don't actually know what it means.

I, on the other hand, found the time between <strike>beers</strike> mission-critical process re-engineering interventions to digest [Martin Fowler's original treatise on refactoring](http://martinfowler.com/books/refactoring.html), so I DO know. 

Sadly, the whole concept of refactoring is borked. Great in theory. Waste of time in practice. 

Let me elaborate:

- As I already said, [I don't like your code.](http://www.devcurmudgeon.com/2010/10/02/i-dont-like-your-code/) Why should I? It's not MY code. Whoever came up with the idea of ego-less programming didn't know many programmers.

- When I say "I" here I really mean *everybody*. "I don't like your code" is just a corollary of "You don't like anyone else's code". Actually, if you're smart you probably don't even like YOUR OWN code. Unless you wrote it very recently and can still remember exactly WHY you <strike>hacked it</strike> had to do it that way.

- Even though I don't like your code, I'm ok leaving it as it is, if it works. Unless I need it to behave differently.

- In other words, if your code isn't *broken*, I'm not going spend any of my time refactoring it.

- Oh, damn. Something changed. *What a surprise*. 

- Now it looks like your previously tolerable code is broken. Even if you refactored it already, you couldn't possibly have anticipated this change, because even though you may be the best coder in the world YOU CAN'T PREDICT THE FUTURE.

- So at this point, refactored or not, [I <b>really</b> don't like your code.](http://www.devcurmudgeon.com/2010/10/02/i-dont-like-your-code/) Not just because you wrote it, but because now it doesn't do what I need it to do.

- The moment I have to make your code do something new, I'll have to re-write some of it. Probably all of it.

- I won't be able to re-factor it first, because I don't like your test code any more than I like the rest of your code.

- In any case, your test framework code is incomplete. Even if *I* wrote the test framework, I already know that I could not possibly have written a *complete* set of tests for anything but the most trivial of programs. So all those passing tests will NOT actually convince me that my refactored code still works. 

- And in the real world, when I play with other people's 'refactored' code, I find bugs that were not present in the original.

- Worse, your test framework doesn't cover the new stuff I need your code to do. Because you didn't predict this. And the changes I need to make will cause your existing tests to fail. Do you really expect me to debug and re-write your tests as well?

- Anyway, even if I *believed* in your test framework, I wouldn't have time for re-factoring, because the BEST I can possibly hope for from following Martin's beautifully expressed guidance would be a chunk of MY code that does exactly what YOUR code already does.

- Why would anyone PAY me to do that?

Oh actually, I KNOW why. If I use a technical sounding name for fiddling with your code, in a way that doesn't actually require me to deliver any additional functionality, maybe management will leave me alone for a while.

While I'm on, maybe I could create a whole set of buzzwords and phrases to convince management I'm really smart? Then I can bat them away with the "cargo cult" argument, just like [Steve](http://www.stevemcconnell.com/ieeesoftware/eic10.htm), Jeff and the rest.

Even better, what about inventing a whole way of working, with its own vocabulary of words that only the initiated can understand? No, I'm not still thinking about <strike>Scrum</strike> <strike>Agile</strike> Steve and Jeff.

I'm actually thinking about [Baserock](http://wiki.baserock.org) :)
