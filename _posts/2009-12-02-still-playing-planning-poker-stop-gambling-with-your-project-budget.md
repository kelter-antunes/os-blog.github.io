---
layout: post
title: Still playing planning poker? Stop gambling with your project budget.
date: 2009-12-02 11:43
author: Robert
comments: true
categories: [agile budget, agile project estimation and budgeting, Dev Zone, outsystems, planning poker]
---
There's a lot of blogging about agile estimating and planning but most, if not all, that I've come across only pertain to after the project has been started.  Further, what is being estimated and planned is for the iterations.  So <strong>how does one define budget for the agile project itself</strong>, specifically a web business application project?  I mean, the cost of the hardware, 3rd party software, facilities, etc. everything except the actual software development cost can be fairly straight forward to budget. <!--more-->

<img class="mt-image-right alignright" style="margin: 0px 0px 20px 20px;" alt="4 aces planning poker.JPG" src="https://www.outsystems.com/blog/wp-content/uploads/2009/12/4-aces-planning-poker1.jpg " width="318" height="212" />

But what about the software development cost?  Using conventional methods or techniques is certainly an option but they do not account for the fact that agile projects tend to cost less when compared to similar projects.  So, perhaps this is not the way to go. Besides, business owners want to know what they're getting for their money and how much it is going to cost them.

At OutSystems, we solved this by taking the following <strong>3 steps</strong>:
<ol>

	<li>First, we work with the business to gather and transform high-level requirements into user stories.  Stories highlight features that detail what the user wants to do (e.g., create, list, search) to specific objects (e.g.customer, store, loan).</li>
	<li>These features are patterns of implementation; it is the patterns that are estimated in hours based on years of experience delivering agile projects successfully and this experience is encapsulated in our OutSystems Agile Network Sizing (ANS) tool (BTW - you can see a demo video <a href="http://www.outsystems.com/demos/DemoScreen.aspx?Movie=Agile-Management--Budgeting-and-scoping-an-agile-project">here</a>).  The tool allows us to set various influencing variables such as number of developers, iteration size, number of user profiles, etc. that enable us to adjust the estimates based on complexity levels.  There are always unknowns during funding and these variables help provide a means to shore up those that may require more attention during the project.</li>
	<li>Given the resources, we are able to calculate what we call the ideal project timeline, complete with sprints and a target go-live date.</li>
</ol>
&nbsp;

You can probably use story points to achieve the same thing assuming you have a common baseline and have equated points to some level of effort which, in turn, equates to dollars.

<strong><span style="font-size: 1.25em;">What if you get funded without this process?</span></strong>

Let's say your project gets funded but you did not use patterns or story points to determine your budget.  You start the project and gather your user stories, prioritize them and the size them.  You conduct your sprints and over the course of say 3 iterations, calculate your average velocity and capacity.  Having your averages, you can calculate the average cost of each iteration and thus the project itself; also, potentially determining when you will run out of budget.  Unfortunately, when using story points and a burndown chart, you still cannot predict with enough certainty when the project will be done. To most stakeholders, stating an approximation or a moving target date is just not acceptable even if you stress the benefits of going agile - early delivery, handling evolving requirements, software that meets specifications, early risk mitigation, etc.

So what do you tell them?  How do you accurately estimate the time and cost it will take and then convince the stakeholders that the project will be done on time and within budget?   Do you give odds when answering when the project will be done?  What do you do if you run out of budget?  Are you gambling with your budget?

Here's the process we've developed:

a) We bootstrap the stories, budget, timeline, sprint definitions from the sizing tool into our project management tool - the OutSystems Agile Network Project (ANP).  The bootstrap process calculates the budget for each iteration based on the overall budget.
b) Each iteration is allocated a budget for development, technical debt, change requests, testing, and sprint review.
c) Once the information is in ANP, we review the stories with the business, prioritize them and even negotiate what goes in an iteration, just like any other agile project.
d) We also break down the user stories into work-items and estimate them (in hours) in conjunction with the developer(s) assigned to complete them.  It is the work-items that we commit to deliver for the sprint.  This helps us ensure that we do not exceed the iteration's budget.

In summary, estimating based on patterns enables us to define the project budget.  Resource estimates and other influencing variables coupled with the budget enables us to provide a project timeline and target go-live date.  This information allows us to manage the project at the sprint level ensuring that we are on target while not exceeding our budget.

What method(s) do you use for estimating project budget and timeline?  What method(s) do you use to ensure you deliver within budget and on time?
