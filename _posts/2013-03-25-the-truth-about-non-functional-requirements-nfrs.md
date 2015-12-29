---
layout: post
title: Functional Requirements and Their Poor Cousins: The Truth About Non-Functional Requirements (NFRs)
date: 2013-03-25 17:58
author: gborrega
comments: true
categories: [Dev Zone]
---
<span style="line-height: 130%; font-family: arial,helvetica,hirakakupro-w3,osaka,'ms pgothic',sans-serif; font-size: 1.5625em;"><b>W</b></span><span style="font-size: 1em; line-height: 130%;">henever anybody says Functional Requirement, I think of princesses. I think of Ariel and Cinderella. I think of how each is central to her story and embodies a specific identity, and then I think of the princess who stands out as a true metaphor for functional requirements - the one who reflects the role perfectly. I think of Snow White.<!--more--></span>

<span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="margin: 10pt auto 20px; text-align: center; display: block;" src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/snow-white-10dwarfs12.jpg" alt="snow-white-10dwarfs.jpg" width="100%" height="auto" /></span>

Snow White is a functional requirement if I ever saw one. She is at once central to her story, its main protagonist, its <i>raison d'etre</i>, yet surrounded by a host of supporting characters - dwarfs - whose roles are necessary for the story to be complete.  No dwarfs, no real story. It's that simple. If a single dwarf is missing, the entire story is compromised. Snow White is compromised.

And it's nearly the same with applications. If an application is the story and Snow White is the functional requirement, then we can think of dwarfs as non- functional requirements (NFRs). If a single NFR is missing from an application then that application is compromised. Deploying a squirrely application is the same as adding maintenance issues and technical debt directly to your application portfolio. Eventually, that application will have to be addressed, those NFRs will have to be added, and the IT department who deployed the app will have to contend with the cost of changing software.

How does this happen? Changing and maintaining software is hard and therefore expensive to do and IT departments are often rushed or underfunded. However, if they are in a 'Just do it' mode then those operational, non-functional requirements that make an application
complete are easy to leave out or are 'forgotten.' The consequences of leaving these NFRs out of an application lead directly to the
aforementioned maintenance problems and increased technical debt.

Here's the list of most common NFRs that we see our customers worrying about:
<table width="630">
<tbody>
<tr>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="margin: 0pt auto 20px; text-align: center; display: block;" src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/Maintainability2.png" alt="Maintainability.png" width="220" height="220" /></span></td>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="margin: 0pt auto 20px; text-align: center; display: block;" src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/portability2.png" alt="portability.png" width="220" height="220" /></span></td>
</tr>
<tr>
<td style="padding-right: 30px;" valign="top">1. <strong>Maintainability</strong>
<p style="text-align: left;">The ease with which the system can be changed, whether for bug fixes or to add new functionality. This is important because a large chunk of the IT budget is spent on maintenance. The more maintainable a system is, the lower the total cost of ownership will be.</p>
</td>
<td style="padding-right: 30px;" valign="top">2.<strong> Portability</strong>
The ease with which software can be installed on all necessary platforms and the platforms on which it is expected to run.</td>
</tr>
<tr>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/reliability2.png" alt="reliability.png" width="220" height="220" /></span></td>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/scalability2.png" alt="scalability.png" width="220" height="220" /></span></td>
</tr>
<tr>
<td style="padding-right: 30px;" valign="top">3. <b>Reliability</b>
<p align="left">The capability of the software to maintain its performance over time. Unreliable software fails frequently, and certain tasks are more sensitive to failure (for example, because they cannot be restarted, or because they must be run at a certain time).</p>
</td>
<td style="padding-right: 30px;" valign="top">4. <b>Scalability</b>
<p align="left">Software that is scalable has the ability to handle a wide variety of system configuration sizes. The nonfunctional requirements should specify the ways in which the system may be expected to scale up (by increasing hardware capacity, adding machines, etc.). Scalability ensures usability for five users or five thousand.</p>
</td>
</tr>
<tr>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/flexibility2.png" alt="flexibility.png" width="220" height="220" /></span></td>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/auditability2.png" alt="auditability.png" width="220" height="220" /></span></td>
</tr>
<tr>
<td style="padding-right: 30px;" valign="top">5. <b>Flexibility</b>
<p align="left">If the organization intends to increase or extend the functionality of the software after it is deployed, that should be planned from the beginning; it influences choices made during the design, development, testing, and deployment of the system. Flexibility is the ease with which the system can be reused, deployed, and tested.</p>
</td>
<td style="padding-right: 30px;" valign="top">6. <b>Auditability</b>
<p align="left">When something goes wrong, you need to understand the root cause of it. So it is normal that auditability is a common NFR. The problem is that you hardly remember to have all the checkpoints in the process, all the exceptions logged, and to ensure that the subsystem to support it does not interfere with your application performance.</p>
</td>
</tr>
<tr>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/documentation2.png" alt="documentation.png" width="220" height="220" /></span></td>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/performance2.png" alt="performance.png" width="220" height="220" /></span></td>
</tr>
<tr>
<td style="padding-right: 30px;" valign="top">7. <b>Documentation</b>
<p align="left">It's hard to keep complex system documentation up to date. Even if you're able to document the initial version of your application, by the time you've finished, the application has changed and its documentation is outdated.</p>
</td>
<td style="padding-right: 30px;" valign="top">8. <b>Performance</b>
<p align="left">The performance constraints specify the timing characteristics of the software. Certain tasks or features are more time-sensitive than others; the nonfunctional requirements should identify those software functions that have constraints on their performance.</p>
</td>
</tr>
<tr>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/security2.png" alt="security.png" width="220" height="220" /></span></td>
<td><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img src="https://www.outsystems.com/blog/wp-content/uploads/2013/03/usability2.jpg" alt="usability.png" /></span></td>
</tr>
<tr>
<td style="padding-right: 30px;" valign="top">9. <b>Security</b>
<p align="left">Integrity requirements define the security attributes of the system, restricting access to features or data to certain users and protecting the privacy of data entered into the software. (<a title="Download HP Fortify OutSystems Case Study" href="http://www.outsystems.com/res/hp-fortify-outsystems-case-study">Download OutSystems Success Story with HP Fortify</a> to learn how we do it)</p>
</td>
<td style="padding-right: 30px;" valign="top">10. <b>Usability</b>
<p align="left">Usability relates to how easily users can learn how to use a system and how efficient they are while using it. Highly usable systems reduce the effort required to read or input data and prevent users from making errors resulting in increased operational efficiency.</p>
</td>
</tr>
</tbody>
</table>
&nbsp;

Like Snow White's dwarfs these NFRs are necessary to completing the story of the application. While you might consider 2 or 3 important NFRs for a project (like performance and security), you'll probably not cover the others extensively enough, or you might miss out on them all together.

And if you do allocate time to deal with them all, when the project schedule slips, the NFRs may be the first thing you'll drop... because no one really sees them, and your team will be looking at the functional requirements instead.

So, whether you plan for NFRs or not, chances are high you won't cover them 100% of the time in your development project. You'll compromise and not think of the whole story - the whole application.

But you should try. You should try to avoid adding technical debt and maintenance nightmares to your future portfolio whenever possible. The cost of change is real, and the moment you deploy your app, you'll have to address its problems.

From your experience what are the NFRs you constantly see developers and project teams dropping most often?

&nbsp;
