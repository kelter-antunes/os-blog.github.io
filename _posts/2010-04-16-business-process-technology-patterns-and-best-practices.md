---
layout: post
title: Business Process Technology - Patterns and Best Practices
date: 2010-04-16 11:32
author: Rodrigo
comments: true
categories: [Dev Zone]
---
Gonçalo Borrêga, from <a href="http://www.outsystems.com">OutSystems</a>, started his session sharing his history with OutSystems BPT: For the last couple of years Gonçalo has been working on a very complex claim handling system, with 708 activities, 501 business rules, and more than 4 million process instances running! And these are processes that run from 2 minutes to more than 2 years!<!--more-->
<div></div>
<div>This claim handling system was refactored from another technology into BPT, using a set of ground rules Gonçalo's team applied.</div>
<div>
<ul>
	<li><b>Know your process:</b> Do deep &amp; early analysis, with the help of your users.</li>
	<li><b>Aim for simplicity: </b>Make it so you can show the process to your users. They will be interacting with the process via de UI!</li>
</ul>
<div></div>
<div><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="text-align: center; display: block; margin: 0 auto 20px;" alt="borrega.jpg" src="https://www.outsystems.com/blog/wp-content/uploads/2010/04/borrega2.jpg" width="520" height="336" /></span></div>
<div>Gonçalo then highlighted the 3 main features he believes differentiate OutSystems BPT from other vendors' solutions:</div>
</div>
<div>
<ul>
	<li><b>Impact Analysis:</b> Process upgrades are possible with the platform! Just do an impact analysis before publishing, and this will help you plan your deployments wisely</li>
	<li><b>The process is close to the data:</b> No need to map the process data to the application data, TrueChange built-in, and an amazing event model are some if the benefits mentioned!</li>
	<li><b>The process is close to the UI:</b> You can place a button in the UI to validate or close activities, and changes are applied to the process in realtime. This allows the UI to guide the users during the entire process.</li>
</ul>
<div>Gonçalo then moved on to share some tips with the audience, based on his experience:</div>
</div>
<div>
<ul>
	<li><b>Empower subprocesses:</b> The platform supports creating really smart sub-processes, that can be reused throughout the application.</li>
	<li><b>Use smart labeling:</b> Labels are shown to end-users in his inbox, so making them clear will really help users navigate the application</li>
	<li><b>Don't do cycles:</b> Unless they really belong to the process, cycles shouldn't be used just to build logic.</li>
</ul>
Gonçalo then prepared the audience for a deeper dive into some advanced patterns. He showed these with the help of Service Studio, and demonstrated to the audience some patterns the platform's BPT is capable of.

</div>
<div></div>
<div>In here he highlighted the ability to customize the end-users' inbox, showing screen shots of a very sophisticated inbox used on a particular project.</div>
<div></div>
<div>The session ended with a big round of applause, and some heavy duty QA that showed the audience was really into the problems and solutions Gonçalo shared today!</div>
&nbsp;
