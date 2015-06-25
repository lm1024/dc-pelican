layout: post
title: Why Should GENIVI Members Contribute, Again?
author: devcurmudgeon
date: 2015/06/23

GENIVI Members need to make attractive, useful software to run reliably in cars for a long time. The amount of software needed is increasing faster than our capacity to bring in extra engineers, and our ability to increase the productivity of the engineers already engaged. Given the economics, automotive organizations tend to favor reuse of existing solutions, since this usually leads to shorter timescales, lower costs and higher reliability.
 
Looking broadly across industries, many organizations and engineers have concluded that the most effective long-term approach for software reuse is Free and Open Source Software (FOSS). It's hard to beat a "license fee" of zero, for solutions that are already being used in a wide range of environments.

In some industries, working with FOSS is a well-trodden path. Major vendors have been using open source for solutions for enterprise, telecoms and mobile for a very long time and have reached some conclusions about what works best. I think the automotive industry is still learning what works best for automotive use cases.
 
To be fair, automotive is really a rather difficult industry, with many demanding constraints: very long product lifetimes, very high reliability and safety requirements, extreme competition on features and price. And the situation is not helped by the dramatic rise in the sheer volume of software required in automotive products over the last few years, leading to levels of engineering cost and complexity way beyond the experience of most automotive decision-makers.
 
I think GENIVI's core challenge is to help its community bridge the knowledge gap, to make best use of what engineers and managers have learned already in other industries. And the "crack in the foundation" is simply that the automotive industry as a whole doesn't yet believe, in its bones, that collaboration and sharing is the best way to deliver in-vehicle software.  Some organizations are hopeful, others are interested, others are running pilot programs, and some are in production, but very few are completely committed to the open source road so far.
 
I'll digress slightly and mention that the Consumer Electronics Linux Forum recently conducted a survey of member engineers to understand what the day-to-day barriers are that stop them from contributing within the open source community. The answers are enlightening, and highly relevant to what we see in the trenches in GENIVI. I'll rephrase the words to make the general point, and attempt to clarify so it makes sense in the automotive context specifically. See  the original [article at LWN](https://lwn.net/Articles/647524/).
 
1. <b>Developing against an old version of the software</b> (54%)
For example, Fred is working on a GENIVI stack from two years ago - patches offered upstream would probably not be useful.
 
2. <b>Work depends on proprietary code</b> (50%)
The work can't be made public.
 
3.  <b>It's too hard</b> (45%)
For example, internal IT makes it difficult to collaborate in the open or follow the contribution process.

4.  <b>Unable to test</b> (41%)
The system Fred is working on is so different from the mainline, it's not clear that any contributions would even work for other teams.
 
5.  <b>Employer does not allow time</b> (40%)
Because contribution is not seen to be commercially justified.
 
6.  <b>Patch not good enough</b> (35%)
Perhaps because the current deadlines are so urgent Fred has no time or budget to improve it.
 
7.  <b>Afraid of rejection</b> (33%)
Aren't we all?
 
Broadly this all boils down to <i>"unless you proactively work with the upstream community, you are unlikely to be contributing patches. Your work is probably not relevant enough or of sufficient quality to be accepted by upstream even if you do try to contribute it."</i>  So the result is that you don't contribute, thus avoiding the cost, pain and time involved in "working with upstream." This makes perfect commercial sense during development, with deadlines looming.
 
Until you realize that you or your colleagues will need to maintain the whole software stack for a very long time, completely adrift from the various upstream teams that developed most of it. <b>Maintaining 100 million lines of code on your own is not much fun, and surprisingly expensive.</b>
 
Automotive has over a century of experience in measuring and improving engineering cost, efficiency and reliability. Software is notoriously hard to measure in detail, but over the long term the clear signals to look at will be:

- total cost of software engineering (in-house and subcontract, development and maintenance) over the lifetime of the product.
- customer complaints, recalls, security breaches and collateral damage.

Unfortunately, we don't yet have clear proof that working in the open and collaborating on solutions over the long-term has delivered better products for automotive at lower cost. It's simply too early to tell.  The numbers aren't in yet. 

But personally I think the evidence from other industries is overwhelming. I know I'm not alone.

(This article was originally published in the June 2015 [GENIVI](http://www.genivi.org) Newsletter.)