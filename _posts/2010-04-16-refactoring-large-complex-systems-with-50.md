---
layout: post
title: Refactoring Large Complex Systems with 5.0
date: 2010-04-16 17:07
author: Rodrigo
comments: true
categories: [Dev Zone]
---
Francisco Menezes, responsible for the Application IT at <a href="http://www.outsystems.com">OutSystems</a>, started by mentioning that OutSystems web applications are all built with the Agile Platform. Over the years, this set of applications got rather large, and refactoring become a challenge.
<div>Francisco pointed out that applications should be designed to scale and potentiate reuse, but due to fast business changes and team rotation, applications grow endemically, which is an impediment to have a one shot "perfect" architecture. <!--more--></div>
<div></div>
<div>Francisco said that he sometimes faces changes from business that demand releases every 2 days, which leads to applications not growing in the most orderly fashion. Another thing that hinders the perfect architecture is the fact that sometimes you need to adapt existing components to fit the existing infrastructure.</div>
<div></div>
<div>At this time Francisco revealed that, from his experience, the 5.0 version of the platform refactors <b>10x faster</b> than 4.2!!! Actually, refactoring turned out to be so easy, his team ended up doing more than initially planned!</div>
<div></div>
<div>Francisco gave a few common scenarios where refactoring is used:</div>
<div>
<ul>
	<li>Separate business logic from UI</li>
	<li>Isolate services for reuse (bottom-up SOA)</li>
	<li>Isolate integrations with 3rd parties</li>
	<li>Replace or adopt a component</li>
</ul>
<div></div>
<div><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="text-align: center; display: block; margin: 0 auto 20px;" alt="refactor.jpg" src="https://www.outsystems.com/blog/wp-content/uploads/2010/04/refactor2.jpg" width="529" height="373" /></span></div>
&nbsp;

Francisco them moved on to explain the recommend architecture for OutSystems' internal applications. This is a layered architecture, with the following components:

</div>
<div>
<ul>
	<li>Website orchestration</li>
	<li>Business processes</li>
	<li>Core business services</li>
	<li>Infrastructure services</li>
</ul>
<div>The recommendation is for top layers to consume whatever the layers below make available, but never the other way around. Unfortunately, applications are not always built with this layered model from day one. Sometimes it is simply impossible to know beforehand how the application is going to grow, which makes refactoring even more of a priority.</div>
<div></div>
<div>Francisco moved on to show the tools improved in the Agile Platform 5.0, to make refactoring as easy as possible. These include:</div>
</div>
<div>
<ul>
	<li>Realtime TrueChange</li>
	<li>Copy &amp; Paste improvements</li>
	<li>Enhanced Find &amp; Replace usage</li>
	<li>Improved Compare &amp; Merge</li>
	<li>New Reference capabilities</li>
</ul>
With these tools, developers can follow the 4 steps to refactoring. For each of the steps, Francisco highlighted the gains he had in productivity just by using 5.0:

</div>
<div>
<ul>
	<li>Isolate and clean the objects to be moved - <b>2x faster</b></li>
	<li>Extract the objects into a new eSpace - <b>5x faster</b></li>
	<li>Generalize the protocol of your new Service - <b>2x faster</b></li>
	<li>Remake references on the consumers - <b>20x faster</b></li>
</ul>
<div>Francisco confided that, although he's talking about 20x faster on that last scenario, he believes sometimes it goes up to <b>100x faster</b>! The new capabilities of 5.0 are really helpful on this scenario!</div>
</div>
<div></div>
<div>To prepare the room for the demo, Francisco gave a short explanation of what he was going to show. In a nutshell, the goal is to move Accounts, a part of a component used by several applications, to a stand-alone component.</div>
<div></div>
<div>In Service Studio, Francisco took advantage of the new features of 5.0 to isolate, extract, and finally remake all the references to Account! Even with the extra time Francisco took to explain the process, the whole refactoring was done in about 10 minutes!</div>
<div></div>
<div>At one point of the process, TrueChange was showing about 500 errors in the application. Using the new capabilities in 5.0, Francisco healed these 500 errors with a single click! That really impressed the audience!</div>
&nbsp;
