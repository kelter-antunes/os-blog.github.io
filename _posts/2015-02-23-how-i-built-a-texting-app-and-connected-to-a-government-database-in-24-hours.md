---
layout: post
title: How I Built a Texting App and Connected to a Government Database - in 24 Hours
date: 2015-02-23 14:31
author: pedroq
comments: true
categories: [Dev Zone, govathon, RAD, sms app, texting app, twilio]
---
I like hackathons. And one of the main reasons I like them is the limited time period the organizers enforce. I take particular satisfaction in delivering production quality and relatively large apps in less than 24 hours. I can do this because a large portion of the work is done with the help of a RAD tool - OutSystems Platform.<!--more-->

This hackathon was called “Govathon.” The City of Atlanta brought together government officials with problems and developers that could craft solutions to these problems. I was one of these developers. Following is my timeline with some short videos showing how I built the app.

<img class="aligncenter wp-image-2303 " src="http://www.outsystems.com/blog/wp-content/uploads/2015/02/Govathon-featured-e14238392461881.jpg" alt="Govathon-featured" width="590" height="241" />
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Friday, 7:00 pm </span>-- Getting started</h4>
The organizers of <a href="http://govathon.com/" target="_blank">Govathon</a> took 30 minutes to present their challenges to the nine teams. Teams assembled themselves around one or several similar ideas. I wanted to pick a project that was useful and would have a chance of being used by the city of Atlanta, and I got intrigued by what Angela Patrick from the building permits office had to say.
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Friday, 8:30 pm </span>-- A mobile app to access government data</h4>
Solving the problem Angela defined would lead to better customer service. People typically call the office to get an updated status on their building permits. There is a web portal but users could not find it easily and were often working at remote locations during the day. Angela wanted a mobile app so people could check their status without having to call the office.
OutSystems has a <a title="OutSystems Platform" href="http://www.outsystems.com/get-started/">fully functional version of their platform in the cloud that is great for personal projects</a>. It is free forever and as long as you don’t need enterprise grade features it is more than enough. I registered and had my development environment up and running in minutes.
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Friday, 9:00 pm </span>-- Integrating with Excel</h4>
<span style="padding-bottom: 20px;">I was given an Excel document with the 60,000 building permits from the last few years, and I quickly created a database inside OutSystems Platform that could hold all the data.</span>

<iframe class="wistia_embed" src="//fast.wistia.net/embed/iframe/wk3bcf3skr" name="wistia_embed" width="100%" height="332" frameborder="0" scrolling="no" allowfullscreen="allowfullscreen"></iframe>
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Friday, 9:45 pm </span>-- The first mobile UI</h4>
<span style="padding-bottom: 20px;">Based on the data, I quickly scaffolded an initial prototype of the user interface using the standard ‘London theme’ that comes with OutSystems Platform.</span>

<iframe class="wistia_embed" src="//fast.wistia.net/embed/iframe/nokjxe96sf" name="wistia_embed" width="100%" height="332" frameborder="0" scrolling="no" allowfullscreen="allowfullscreen"></iframe>
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Friday, 10:30 pm </span>-- Going home to sleep</h4>
<img class="aligncenter size-full wp-image-2357" src="http://www.outsystems.com/blog/wp-content/uploads/2015/02/sleeping1.png" alt="sleeping" width="500" height="173" />
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Saturday, 8:30 am </span>-- <span style="padding-bottom: 20px;">Multichannel apps: Developing a text interface with Twilio</span></h4>
While getting dressed, I thought about the real-use scenario of this app. Adoption rates of mobile apps are ridiculously low if the real usage scenario is misunderstood. I wondered if a texting interface to query the database would yield better adoption rates. <a href="http://www.twilio.com" target="_blank">Twilio</a> to the rescue!

<img class="alignnone wp-image-2358 size-full aligncenter" src="http://www.outsystems.com/blog/wp-content/uploads/2015/02/govathon-screenshot-mobile-device-e14240869589491.jpg" alt="govathon-screenshot-mobile device" width="590" height="361" /> Twilio is a telephony service, that among other things, enables apps to send and receive text messages. I integrated Twilio with my app using the REST capabilities of OutSystems Platform.
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Saturday, 9:30 am </span>-- Twilio integration using a service callback</h4>
<span style="padding-bottom: 20px;">This sophisticated integration was made simple with OutSystems Platform. I created a Twilio account, which gives me a phone number. Any text message sent to that phone number generates a callback into my app. Check out how fast I did it.</span>

<iframe class="wistia_embed" src="//fast.wistia.net/embed/iframe/7vvaombu3d" name="wistia_embed" width="100%" height="332" frameborder="0" scrolling="no" allowfullscreen="allowfullscreen"></iframe>
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Saturday, 10:00 am </span>-- Publishing and running the app</h4>
<span style="padding-bottom: 20px;">This is how it works. Send a text message (SMS) to the phone number, then the app fetches the data from the database and sends the result back by text.</span>

<iframe class="wistia_embed" src="//fast.wistia.net/embed/iframe/uqbm2hylxm" name="wistia_embed" width="590" height="332" frameborder="0" scrolling="no" allowfullscreen="allowfullscreen"></iframe><script src="//fast.wistia.net/assets/external/E-v1.js" async=""></script>
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Saturday, 10:30 am </span>-- Live integration with the permit database service</h4>
<span style="padding-bottom: 20px;">I was done. I headed down to Atlanta Workforce Development headquarters and had some time before I was to demo and present my app at 3:00. But I could not resist some enhancements! The permit database is supported by <a href="http://www.accela.com" target="_blank">Accela</a>, and they have a great <a href="https://developer.accela.com/" target="_blank">public REST API</a>. <a href="https://twitter.com/mheadd" target="_blank">Mark Headd</a> was nice enough to send me a couple of request/response examples that I fed into OutSystems Platform. Ten minutes later, I was able to connect my texting app to the live data of building permits of Atlanta.</span>

<iframe class="wistia_embed" src="//fast.wistia.net/embed/iframe/lepbhhbjjn" name="wistia_embed" width="590" height="332" frameborder="0" scrolling="no" allowfullscreen="allowfullscreen"></iframe>
<h4 style="padding-top: 25px; padding-bottom: 15px;"><span style="color: #cc0000;">Saturday, 3:00 pm </span>-- Winning!</h4>
<a href="http://www.outsystems.com/blog/wp-content/uploads/2015/02/Govathon-1st-Place1.jpg" target="_blank" rel="attachment wp-att-2381"><img class="padding-right:20px alignleft wp-image-2381 size-thumbnail" src="http://www.outsystems.com/blog/wp-content/uploads/2015/02/Govathon-1st-Place-150x1501.jpg" alt="Govathon-1st-Place" width="150" height="150" /></a><a href="https://twitter.com/eklementich" target="_blank">Eloisa Klementich</a>, co-founder of Govathon, announced the winners. Citing innovation and growth as a primary objective of the City, she was pleased to name my Building Permitting app as the winner of the fourth annual Govathon!

Now residents and businesses can check the status of their building permit applications in real time!

&nbsp;

RAD platforms work. OutSystems Platform allowed me to deliver a working SMS app with live integration in less than 24 hours - with some sleep included :)

&nbsp;

&nbsp;
