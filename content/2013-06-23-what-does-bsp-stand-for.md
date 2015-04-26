layout: post
title: What does "BSP" stand for?
author: devcurmudgeon
date: 23/06/2013

During a <strike>late-night drinking session</strike> technical discussion this week there was confusion about the meaning of "BSP" for Linux and Android. 

Some folks think BSP stands for "Board Support Package". 

But, as with [SCRUM](http://www.devcurmudgeon.com/2010/08/28/software-chaos-ridiculously-under-managed/), the popular view is wrong.

In the real world, BSP means <b>Bull Shit Project</b>.

BSPs are a source of extreme pain. A huge waste of time and money.


+ Getting permission to know the BSP even existed in the first place probably required a hard-core NDA, even though most of the important files turn out to be GPL.

+ Then there was a struggle to find the BSP itself, because getting a login/password for the "secure" extranet took forever followed by weeks spent hunting around for the right version of the BSP amongst all the other <strike>crap</strike> premium content.

+ It probably came as a <strike>zip file</strike> tarball containing <strike>a load of junk from the developer's source directory that day</strike> a full snapshot of the kernel<strike> hacked together two years ago during a caffeinated rush to hit some demo deadline</strike>.

+ It was probably developed for the chipset vendor by <strike>monkeys</strike> experts who <strike>stole</strike> reused existing Windows code before getting <strike>fired</strike> rushed on to their next project.

+ The custom stuff that the <strike>monkeys</strike> experts developed probably has their organisation's name in the source files, even though they did it in secret, as a work-for-hire, so the SoC vendor is the actual copyright owner. 

+ Those same source files probably <b>don't state that the code is GPL</b>. Maybe the <strike>monkeys</strike> experts <strike>had no clue about licenses</strike> figured all the downstream developers could work out the license for themselves.

+ And now the cost of backporting patches to that two-year old kernel gets bigger every day until finally, someone will *have* to port to a newer one. 

+ And then the nightmare will repeat. Just with a newer BSP, that quickly becomes old and bitrotten, like the original. 

That's the real world today. We need to <b>change</b> this world.

So here's an idea that bubbled up during the <strike>late-night drinking session</strike> technical discussion I mentioned earlier. 

Even though [LOC is a terrible metric](http://www.devcurmudgeon.com/2013/06/02/the-worst-metric/), it could help us to solve the BSP problem once and for all.

It's simple. <b>We need to minimize the BSP LOC</b>. 

Repeat after me... the target is ZERO BSPLOC. I don't care if you pronounce that bee-ess-pee-ell-o-cee or bee-sploc or something else. 

But I'm sure the target is ZERO.

No lines of code in the BSP. 

This is not some devCurmudgeon pipedream. Linaro, Intel, Samsung, Calxeda and others are pushing this way already. 

Everything in mainline. 

That way, we know for sure that the code the <strike>monkeys</strike> experts wrote was reviewed and accepted by real Linux hackers. And that means there's a realistic chance it will continue to work as Linux moves forward.

