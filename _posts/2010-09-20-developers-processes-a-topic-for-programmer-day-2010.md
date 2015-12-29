---
layout: post
title: Developers & Processes - A topic for Programmer Day 2010
date: 2010-09-20 10:21
author: gborrega
comments: true
categories: [Agile Platform, Agile tools, Application Development, BPM, BPT, Business process technology, Caixa Seguros, Platform in Action]
---
<div>Following <a href="https://www.outsystems.com/blog/aboutagility/2010/09/celebrating-programmer-day-with-warp-development.html">Rodrigo's last post</a> on Caixa Seguro's <a href="http://www.programmerday.info/">Programmer Day</a>, I would also like to share with you my session on OutSystems' Business Process Technology. The Caixa Seguros team relies pretty heavily on Business Process Management, and they were eager to learn more about our capabilities and experience!</div>
<div>As such, I was pleased to show them how OutSystems' approaches with the application of BPM technologies and implementations for their specific industry: Insurance - Policy and Claims handling.</div>
<!--more-->
<div></div>
<div>I started by presenting some common concepts we felt were important to address with our BPM approach in the Agile Platform, we call this Business Process Technology or BPT for short.  The key concepts are:</div>
<div></div>
<div>
<ul>
	<li><b>Long lived processes:</b> requiring process instances to be upgraded as new laws, conventions, or procedures are brought in.</li>
	<li><b>Strong cohesion with line-of-business applications:</b> processes are always supported by a business application (or more than one), and this application should work seamlessly with the process.</li>
	<li><b>Big benefits in the end: </b>processes allow every organization to increase operational performance, especially those with clear procedures in their activity. Just getting everyone to know what they're supposed to do improves performance dramatically; according to Gartner, simply having the workflow users should follow on the wall leads to a 12% improvement on productivity. The set of monitoring tools and KPI collection provided by BPM engines brings focus on the need to optimize, and provides leads on how we can optimize it.</li>
</ul>
</div>
<div><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="text-align: center; display: block; margin: 0 auto 20px;" alt="BAM_Screeshot.png" src="https://www.outsystems.com/blog/wp-content/uploads/2010/09/BAM_Screeshot2.png" width="508" height="140" /></span></div>
<div>The next step was to point out the main challenges faced when setting up a BPM initiative to work with an existing - or new - set of applications that support the same goal. From real field experience, we identified the following set of challenges as the most relevant:</div>
<div></div>
<div>
<ul>
	<li><b><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-right" style="float: right; margin: 0 0 20px 20px;" alt="BPM_Glasses.png" src="https://www.outsystems.com/blog/wp-content/uploads/2010/09/BPM_Glasses2.png" width="150" height="111" /></span>Separation from User Interface:</b> having a process that redirects users to perform manual activities on an application is troublesome for the single fact that they live and are implemented in a separate environment from the application.</li>
	<li><b>Complex API integration:</b> the requirement to plug-in a process' inbox to an application and having the application ignite and advance the processes requires usage of the engine's API, which are not well integrated with the application and are usually hard to extend by the application developers.</li>
	<li><b>Intermediate domains:</b> When processes and applications are supported by different platforms, they still need to share data between them. This leads to non-business related and error prone developments of intermediate data dictionaries, being produced and consumed by each other. When either the application or the process change, these dictionaries also need to be refactored.</li>
	<li><b>Upgrading existing processes:</b> as process definitions change, thousands or millions of running process instances need to be upgraded to the new definition.</li>
	<li><b>Distinct life-cycle between application and process:</b> This leads to inefficiencies in both the application and the process, and can even lead to inconsistencies in the several releases integrations.</li>
</ul>
</div>
<div>With this in mind, I picked a real application used for project management and did a live demo creating a process live during my presentation. The fact that in the Agile Platform, our BPT is implemented as a layer on top of the application removes all the problems mentioned above. While the process is being built, the Agile Platform's <a href="http://www.outsystems.com/agile-platform/true-change/">TrueChange</a> engine detects changes in the entity model and fixes them immediately throughout the process, discarding the need for the tiresome task of creating intermediate data dictionaries. It was also clear that having the process near the application allows doing a lot of neat things, such as a chat like interface where a user leaves his comments on an activity and reassigns it to another user, all in the context of a common application interface.</div>
<div></div>
<div>During the session I showed the audience how business users could check the performance of the just created process via the Agile Platform's built in Analytics application. Right in the session I demonstrated how you are able to immediately provide process feedback using our <a href="http://www.outsystems.com/agile-platform/change-management/">Embedded Change Technology</a>. During the session I actually implemented the feedback, and made a change to the process right on the stage. The change required me to upgrade the process, which brought up the clear advantages of having an integrated Impact Analysis before putting new versions into production. This allows operations teams to easily measure the impact of changes in the process, before they are actually deployed.</div>
<div></div>
<div>By the end of the presentation, I believe everyone saw the advantages of having a platform that fosters a common development life-cycle between application and processes. This makes it much easier to build a process that leads the users through their tasks in the application, definitely bringing the Business and IT together in one same purpose: business performance.</div>
<div></div>
<div>Want to learn more? Don't miss our <a href="http://www.outsystems.com/training-and-certification/classroom/courses/business-process-technology/">BPT workshop</a> taking place on October 11th in Lisbon!</div>
&nbsp;
