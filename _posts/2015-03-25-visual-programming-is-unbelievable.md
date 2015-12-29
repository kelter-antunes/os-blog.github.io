---
layout: post
title: Visual Programming Is Unbelievable... Here’s Why We Don't Believe In It
date: 2015-03-25 12:09
author: tiago
comments: true
categories: [Uncategorized, visual programming]
---
<img class="alignnone size-full wp-image-2749" src="http://www.outsystems.com/blog/wp-content/uploads/2015/03/blog1.jpg" alt="blog1" width="590" height="256" />
Visual programming has been an unfulfilled prophecy for years. As so many other areas, like virtual reality, artificial intelligence, or speech recognition, when the hype was high, the underlying technology wasn’t there yet.

But that was not its only problem...<!--more-->
<h5 style="padding-top: 10px"><strong>Several Misfires</strong></h5>
For visual programming, the hype peaked in the early 90s with CASE tools. And, as with all trends ahead of their time, the repercussions of its failure were years of underinvestment, little innovation, and lingering skepticism.

UML (Unified Modeling Language), with its promise of bringing sanity to object-oriented programming, hasn’t helped either, although much of its faults were due to the underlying complexities related with inheritance.

And even more recent trends, like Business Process Modeling, probably did more harm than good in giving credibility to this area.
<p style="text-align: center"><img class="wp-image-2736" src="http://www.outsystems.com/blog/wp-content/uploads/2015/03/blog2.png" alt="CASE tools, UML, and BPM all failed to deliver on their promises" width="400" height="92" />
<span style="line-height: 1.5;color: #808080">CASE tools, UML, and BPM all failed to deliver on their promises</span></p>

<h5 style="padding-top: 10px"><strong>No Silver Bullet</strong></h5>
In his seminal <a title="No Silver Bullet" href="http://en.wikipedia.org/wiki/No_Silver_Bullet" target="_blank">No Silver Bullet</a> paper, Fred Brooks stated that there is no single development which, by itself, promises one order-of-magnitude improvement in productivity, because technology complexities would decrease, but requested features would not.

Like Moore’s law on hardware, the first part of that sentence proved to be prescient almost 30 years ago. What Brooks might have missed is that this would make room for too many directions in software development, often making us move in circles, instead of forward.

An example is the explosion of the number of languages, idioms and practices, sometimes with opposite approaches (e.g. strongly/weakly typed, client-server/server, all the different new JavaScript frameworks, etc...). Non-functional requirements, like scalability or security, and new expectations, like mobile and user experience, have only made things harder.

<img class="aligncenter size-full wp-image-2737" src="http://www.outsystems.com/blog/wp-content/uploads/2015/03/blog3.png" alt="blog3" width="100" />

All this complexity opens space for an approach that would allow developers to focus more on delivering real value. Visual programming, with its higher level abstraction, could be the champion for this approach and become the productivity silver bullet we’ve been looking for.

So why hasn’t it yet?

Because visual languages have a fundamental set of problems:
<h5 style="padding-top: 10px"><strong>Visual Languages Aren’t Extensible</strong></h5>
This is probably the capital sin of visual languages. They allow you to do a limited set of things easily, but edge cases are far too difficult, or even impossible to achieve. Tools should give us more power, instead of limiting us.
<h5 style="padding-top: 10px"><strong>Visual Languages Generate Slow Code</strong></h5>
Every developer who has faced performance problems knows how hard they are to diagnose and overcome. Visual languages are leaky abstractions, often generating slow code which is impossible to optimize.
<h5 style="padding-top: 10px"><strong>Visual Language Tools Can Be Terrible</strong></h5>
We live and breathe in our IDEs (Integrated Development Environments). When they are poor, they can make our lives miserable! Visual languages and IDEs should be designed together: our love or hate for a language is a direct measure of our love or hate for its tools.
<h5 style="padding-top: 10px"><strong>Visual Languages Lock You In</strong></h5>
Any technology decision brings a level of lock in. The fear of being locked into a dead-end is justifiable, given that most visual languages generate unreadable lower level code, only target niche segments, are supported by suicidal startups, or haven’t left the research lab yet (where amazing recent work, like <a title="Bret Victor's" href="http://worrydream.com/MediaForThinkingTheUnthinkable/" target="_blank">Bret Victor’s</a>, is being done). Real success stories, of people using it in large projects, are still rare, and these communities are still growing.
<h5 style="padding-top: 10px"><strong>You Are Neurologically Programmed to Reject It</strong></h5>
The problems in the previous sections are serious and, as visual language architects, we know it’s our responsibility to continue our work to address them, removing these limitations.

But there are deeper reasons why you don’t trust visual languages:

<img class="aligncenter size-full wp-image-2738" src="http://www.outsystems.com/blog/wp-content/uploads/2015/03/blog4.png" alt="blog4" width="100" />

The first is related to our love for complexity. Although we might say otherwise, we all do, according to the father of usability, <a title="Don Norman" href="http://en.wikipedia.org/wiki/Don_Norman" target="_blank">Don Norman</a>. Take musical instruments, for instance: musicians love them because they are hard to master. Think about legislation. Or even language: most poetry is hidden under complex sentences and words. We love the intellectual challenge of thinking difficult thoughts. Your mind is probably doing it right now, agreeing with these ideas, or checking if there is anything wrong or missing in them.

We need, however, to be careful with this, as we create deep moats against the rest of the world, and that brilliant xor swap algorithm I’ve coded today may be somebody else’s nightmare next year.

Like Steve Jobs said: “Simple can be harder than complex. But it’s worth it.”

The second reason is even more primitive: it’s fear of change. We take the time to acquire some expertise, and suddenly it seems our old weapons are no longer needed. But we’re seeing it wrong: our weapons are not to be able to do a malloc, or pointer arithmetic; they are to be able to divide a problem into smaller parts, to understand the process of iterating on its solution, to detect strange code smells, to discuss a diagram on a whiteboard, to refactor systems into better architectures.

Those are our real weapons, the ones we’ve been sharpening for years, weapons that, with higher level languages, become even more deadly to any problem that might cross our path. Fear not: a great developer will always be more valuable than any tool he works with.

And let's face it: there’s also social acceptance. We were here first, we bought the debut albums, we'd never be caught listening to the sellouts that make it easy for everyone.
<h5 style="padding-top: 10px"><strong>We’ve Been Here Before</strong></h5>
Because of these instinctive reactions, anything that aims to democratize computing is met with skepticism. HyperCard, Delphi, Visual Basic, COBOL. We, the “real” developers, are too quick to point out their faults, and mock them with no mercy until they die, instead of helping them improve. Even JavaScript almost had that same fate during the DHTML days.

<img class="aligncenter size-full wp-image-2739" src="http://www.outsystems.com/blog/wp-content/uploads/2015/03/blog5.png" alt="blog5" width="100" />

There is, however, an analogy that might better show us the future: The shift from text operating systems, like Unix and MS-DOS, to graphical user interfaces, like Mac or Windows, which suffered pushback from several computer experts at the time.

That evolution, which seems so inevitable today, brought us better graphic cards - which lead to better games, brought us the world wide web, brought us smartphones.

Can you imagine a world without these unbelievable things?
<h5 style="padding-top: 10px"><strong>So, Are We Finally Ready For It?</strong></h5>
Not sure: you may not, or you may feel we’re not - it’s fair either way. But try to understand your biases, and don’t be afraid to give visual languages a shot: there are several organizations like mine, in different domains, challenging the way software is traditionally delivered, and pushing forward the state of the art.

And even if, after trying them out, you still don’t see the bright future of visual programming, that’s fine: consider keeping an open mind and come back later, otherwise you might just end up in the wrong side of history.

&nbsp;
