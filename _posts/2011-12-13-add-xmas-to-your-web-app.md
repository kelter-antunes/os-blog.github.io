---
layout: post
title: Add a bit of Xmas to your web app
date: 2011-12-13 12:40
author: Rodrigo
comments: true
categories: [christmas, custom development, Dev Zone, web app, Web Application]
---
We're already deep in the holiday season, but it's never too late to <b>add a bit of Xmas spirit to your Web Application</b>!

I thought about adding Xmas lights, flying reindeers, working elves... but it seems to me that for an Enterprise Web Application something a bit subtler was in order.

<!--more-->

So I ended up just putting in a bit of snow on the Sales application:
<p align="center"><object width="480" height="305" classid="clsid:d27cdb6e-ae6d-11cf-96b8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=6,0,40,0"><param name="allowFullScreen" value="true" /><param name="allowscriptaccess" value="always" /><param name="src" value="http://www.youtube.com/v/Y6xnAa268O0?version=3&amp;hl=en_US&amp;rel=0" /><param name="allowfullscreen" value="true" /><embed width="480" height="305" type="application/x-shockwave-flash" src="http://www.youtube.com/v/Y6xnAa268O0?version=3&amp;hl=en_US&amp;rel=0" allowFullScreen="true" allowscriptaccess="always" allowfullscreen="true" /></object></p>
<p align="center"><span style="font-size: 0.8em;">Check the video to see snow in action, or visit the <a href="http://www.outsystems.com/network/" target="_blank">OutSystems Network</a> to see it live in a real web page!</span></p>
If you're using the <a href="http://www.outsystems.com/agile-platform/">Agile Platform</a> and want to add some snow to your app, here's what you need to do:
<ol>
	<li><a href="http://www.outsystems.com/NetworkSolutions/ProjectDetail.aspx?ProjectId=273" target="_blank">Get the "Xmas" component</a> from the OutSystems Community</li>
	<li>Reference the component from your web app</li>
	<li>Drag the "LetItsnow" block to a particular page, or to the footer if you want snow on all pages</li>
	<li>Click 1CP, sit back, enjoy your eggnog, and let it snow!</li>
</ol>
If you're not using the Agile Platform, there's a bit more work involved...
<ol>
	<li>Get the Javascript file from <a href="http://www.schillmania.com/projects/snowstorm/" target="_blank">this site</a></li>
	<li>Place the Javascript on all your front end servers</li>
	<li>Edit your pages and look for the <tt>&lt;head&gt;</tt> section</li>
	<li>Add the line <tt>&lt;script src="snowstorm.js"&gt;&lt;/script&gt;
</tt></li>
	<li>Customize the snow with a bit more Javascript
<tt>&lt;script&gt;
snowStorm.snowColor = '#cccccc';
snowStorm.snowStick = false;
snowStorm.animationInterval = 75;
&lt;/script&gt;
</tt></li>
	<li>Make sure you didn't break anything!</li>
	<li>Follow the "move to production" checklist (if you have one)</li>
	<li>Send the changes to your ops team and wait for them to move it to production... hopefully that will happen before Xmas! :)</li>
</ol>
<div>Have a snowy Merry Xmas!</div>
