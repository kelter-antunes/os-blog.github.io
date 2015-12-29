---
layout: post
title: Developer Diary: Justin James integrates & deploys an application with the Agile Platform
date: 2010-06-25 08:56
author: Rodrigo
comments: true
categories: [application deployment, application integration, Dev Zone, Justin James Developer Diary, outsystems, Tech Republic]
---
I just read <a href="http://techrepublic.com.com/5213-6257-0.html?id=2926438&amp;allowContact=false&amp;tag=content;leftCol&amp;authId=jKGpJgFbxmTfww7HtEwv4Ctx27vd3yxXccLXt4mi5lmsbRmyEv44SlY4hN2rU+9h">Justin James</a>' most recent diary entries <a href="http://blogs.techrepublic.com.com/programming-and-development/?p=2660&amp;tag=content;leftCol">#4</a>&amp; <a href="http://blogs.techrepublic.com.com/programming-and-development/?p=2708&amp;tag=content;leftCol">#5</a>, where he continues to develop his Rat Catcher web application; his next challenge - to integrate custom code, he'd already developed, into the <a href="http://www.outsystems.com/agile-platform">Agile Platform</a>. As Justin said, "I was not worried -- after all, I knew that Integration Studio would let me hook up my application to this code."

<!--more-->

I thought I'd share some key learnings and highlights from these two journal entries.
<span style="font-size: 1em;">(BTW, If you missed the previous entries of Justin's diary check this <a href="https://www.outsystems.com/blog/aboutagility/2010/05/a-developer-diary-justin-james-on-the-agile-platform-service-studio.html">previous post</a> on the About Agility blog.)</span>
<div style="padding-top:20px;"><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="text-align: center; display: block; margin: 0pt auto 20px;" alt="JJ4 pic.jpg" src="https://www.outsystems.com/blog/wp-content/uploads/2010/06/JJ4%20pic1.jpg" width="508" height="255" /></span><b>Integrating Web Services</b></div>
<div>Turns out Justin's code uses some advanced patterns, and although Integration Studio did its part and "was successful at a technical level," Justin opted to use another form of integration: Web Services. As soon as Justin made his code available as a web service "it was a cinch to point Service Studio to the deployed Web service." Well, Justin did find a little bug, but this was a great opportunity for him to connect with the OutSystems <a href="http://www.outsystems.com/Network/">community</a> for help and guidance, and we're really happy that he thought "it was a great experience"!</div>
<div  style="padding-top:20px;"><b>Deploying Rat Catcher</b></div>
<div>With all the pieces in place, it was now time to deploy the first public version of <a href="http://ratcatcher.titaniumcrowbar.com/RatCatcher/">Rat Catcher</a>. Justin has a pretty elaborate infrastructure, and the experience he documents in the diary entry will surely help people with similar setups. Nice to hear that installation was a breeze, since "the team did an amazing job with version 5 and getting the install to be smooth and easy."</div>
<div></div>
<div  style="padding-top:20px;"><b>Doing things the hard way - but learning...</b>
After configuring the Agile Platform, all that was left was deploy the application. Justin actually did this the hard way; he deployed one component at a time... but I was really happy to see that he learned all about the OutSystems solutions, so he is now able to quickly move all components to production at once, while keeping version records so he can rollback to old versions if needed.</div>
<div>I'm looking forward to the next five installments to hear about his continued experience with the platform, and hope you're following along too. What do you think of Justin's experience so far?</div>
<div></div>
