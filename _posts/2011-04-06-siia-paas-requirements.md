---
layout: post
title: SIIA PaaS Requirements
date: 2011-04-06 14:26
author: mwj
comments: true
categories: [cloud, Dev Zone, PaaS, SaaS, SIIA]
---
<div>The Cloud...  It's like teenage sex. Everyone is talking about it - but no one is really doing it. Also like teenage sex sooner or later you will. Thus while the hype is driving us all a bit crazy we have to pay some attention to how this will play out as sooner or later we will get involved. Like most things in the technology world, the concepts are not all that new.</div>
<div></div>
<div>What has changed is the terminology and more importantly <b>the availability of the technology has gotten better</b>. This makes things more accessible, usable, etc. For example, it was not but a few years ago that you still used a phone line and wire to connect to your email when traveling on business. How we forget the good ole days and thank someone for wireless access. In the cloud we are making access to virtualized servers, data stores and the needed services to manage them available under a utility model - <b>you only pay for what you use</b>.<!--more--></div>
<div></div>
<img class="mt-image-right" style="float: right; margin: 0 0 20px 20px;" alt="siia-clipboard.png" src="https://www.outsystems.com/blog/wp-content/uploads/2011/04/siia-clipboard2.png" width="220" height="310" />
<div>So the cloud. OK, I think we all get the basics of having a virtual data center and the notion of a utility model for getting access to a remote infrastructure. Being able to offload some of the operational costs associated with managing your infrastructure is promising. What I see as the real challenge is how all of this will impact the more difficult side of IT, <b>application development and management</b>. This is where we create business value and where the cloud has some maturing to do before its full promise will be recognized.</div>
<div></div>
<div>So what about application development in the cloud - how are you going to get it done? Well there is SaaS which is effectively the cloud's 'package' application market. This is good for those commodity processes where you can buy a package. But for the differentiating processes where you have to build an application we have to look at things like PaaS or platform as a service. To this end I wanted to share a snippet from a recent <a href="http://siia.net/aatc/2011/">SIIA article</a> that outlined their thinking on the minimum requirements you'll need to provide a "Best-in-Class" Platform-as-a-Service (PaaS) offering:</div>
<div></div>
<div>
<ul>
	<li><b>Multi-tenant architecture -</b> common technical resources and code instance for multiple client companies.</li>
	<li><b>Customizable/Programmable User Interface -</b> support the creation of high-flexible user interfaces without the need to write complex code.</li>
	<li><b>Unlimited Database Customizations -</b> provide ability to easily modify/extend the data model (i.e. construct objects, define relationships, specify validation rules/permissions) via a "point-and-click" declarative" environment.</li>
	<li><b>Robust Workflow capabilities -</b> engender process automation by providing "point-and-click" tools to easily define workflow processes and specify business rules.</li>
	<li><b>Granular permissions model -</b> multi-level control over security/sharing within/across applications and platform components.</li>
	<li><b>Flexible services-enabled integration model -</b> enable seamless integration of "cloud" application data and functionality via a flexible web services enabled integration model.</li>
	<li><b>Analytics layer -</b> enhanced ability to leverage aggregated data across companies and applications for analytics.</li>
	<li><b>Integrated content library -</b> common elements that extend the core application feature set, improve info-sharing and speed up go to market time.</li>
</ul>
</div>
<div></div>
<div>This list sounds reasonable. I would push back on the need for multi-tenancy.  Why?  If I am an enterprise IT shop wanting to build applications for my business - I don't share my application software thus this need is not important. I would also add the requirement to have my PaaS give me <b>the option to deploy any new application on premise as well as in the cloud</b> - you never know when something is going to force you to move your data and processes to a more secure setting. Check out the eBook the OutSystems team put together on PaaS <a href="http://www.outsystems.com/offer/avoid-paas-development-traps/">here</a> and let me know what you are considering for application development in the cloud.</div>
&nbsp;
