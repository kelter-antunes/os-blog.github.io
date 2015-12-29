---
layout: post
title: "The Big Move: How We Migrated Core Applications to the Cloud"
date: 2012-03-19 12:54
author: acacio
comments: true
categories: [application in the cloud, cloud, cloud application, cloud migration, migrate to cloud, Platform in Action]
---
<div>For the last couple of months, it seemed a few of our core applications weren't behaving as well as they should... Some applications were running a bit slow, and we experienced connectivity problems related to our ISP.</div>
<div>This was serious because these are core systems running on top of the <a href="http://www.outsystems.com/agile-platform/">Agile Platform</a>, and include our website, our community, our partner network, our product management tool, and a host of other internal applications.<!--more-->Since responsiveness and availability are two fundamental traits of a great app, we had to do something about it. We decided to move our infrastructure to the cloud, in particular to <a href="http://aws.amazon.com/ec2/">Amazon EC2</a>. And because these were core apps, we had to do it with minimum downtime and guaranteeing all the needed accesses.</div>
<div style="padding-top: 1.25em;"><span style="font-size: 1.25em;"><b style="color: #1f5ba4;">The old infrastructure</b></span>
The infrastructure we wanted to move to Amazon was made up of two separate OutSystems production environments - we decided not to move the development and QA environments. These environments and their applications were built using a Service Oriented Architecture to communicate with each other, and to integrate with third-party apps like <a href="http://www.pardot.com/">Pardot</a> and <a href="http://www.salesforce.com/">Salesforce</a>. Another part of the challenge was that these systems are used by internal OutSystems' applications, deployed in different infrastructures - including business-critical integrations with the R&amp;D process. This raised some security concerns and some challenges on how to keep supporting these integrations with minimal changes to the architecture.</div>
<div><span class="mt-enclosure mt-enclosure-image" style="display: inline;"><img class="mt-image-center" style="text-align: center; display: block; margin: 0 auto 20px;" alt="cloud-application-migration.png" src="https://www.outsystems.com/blog/wp-content/uploads/2012/03/cloud-application-migration2.png" width="526" height="350" /></span></div>
<div style="padding-top: 1.25em;"><span style="font-size: 1.25em;"><b style="color: #1f5ba4;">The new setup</b></span>
Since the machines about to be replaced were near retirement, and because in Amazon we can add machines as needed, we decreased the number of servers from 5 front-ends to 3. We have an additional machine with SQL Server and, at the time of writing, all machines are m1.large (2CPU, 5 Amazon ECU, 7.5GB RAM). To distribute load between the Amazon front-ends, we are using Amazon Load Balancer.</div>
<div></div>
<div style="padding-top: 1.25em;"><span style="font-size: 1.25em;"><b style="color: #1f5ba4;">Preparing for the big move</b></span>
In order to perform the move, we used an approach similar to the hot-standby approach suggested to our Agile Platform customers. The idea is to setup an infrastructure on the cloud, and use the disaster recovery option to move control to this new infrastructure. For this, we had to:
<ol>
	<li>Make sure all users were accessing the in-house systems from the outside network, just to make sure that everything that was needed was in fact available. This was good to identify certain content that needed to be accessed via HTTPS, for security reasons;</li>
	<li>We had to set up a database mirror for the SQL Server database. This was a big step, considering we moved 120Gb to Amazon -- a 2 day transfer! And since our internal infrastructure kept working, by the time it was done we had an extra gigabyte to move. Also, being two remote installations of SQL Server, we had to setup a secure mirror with certificate authentication -- which has its own tricks as well;</li>
	<li>We then installed the front-end servers in the cloud, and set them up to connected to the in-house database. This was easy, since OutSystems already provides Amazon images. The trickier bit was to ensure a secure connection with our internal systems, something we achieved using OpenVPN;</li>
	<li>Finally, we tested to make sure everything was working. We used some automated test scripts, and took the chance to identify dependencies with internal systems. To fix these dependency issues, we had to move some components back to the internal datacenter, and connect everything using webservices on top of HTTPS. Fortunately, this is really easy to do with the Agile Platform as it makes building webservices and delivering a service oriented architecture easy and fast! The only thing we couldn't test was performance... after all, the database was still in our datacenter, 3 thousand miles from the front-ends.</li>
</ol>
</div>
<div style="padding-top: 1.25em;"><span style="font-size: 1.25em;"><b style="color: #1f5ba4;">Pull the switch!</b></span>
With all the preparation done, it was time to go full cloud. Here's what we did:
<ol>
	<li>We started by turning off the in-house systems. No problem here, just had to put an unavailable page and stop the OutSystems' Agile Platform and IIS.</li>
	<li>Next, we brought the cloud database server up. We were a bit worried with the time it would take to resync our SQL Server mirror after the rotation, but it only took about a minute. It took less than 5 minutes to have everything ready and to configure.</li>
	<li>After that, we reconfigured the Agile Platform to use the cloud database. No problems there, we just had to launch the configuration tool, modify the database settings, and restart the platform.</li>
	<li>Finally, we had to change the DNS servers to point to the new infrastructure location.</li>
</ol></div>

<span style="font-size: 1.25em;"><b style="color: #1f5ba4;">The results</b></span>
In the end, we definitely achieved our goal: Our core applications are running faster, and in time we'll be able to measure how connectivity improved since moving to the cloud.

It's also amazing how fast we were able to make the move. The procedure took 4 hours, but it could've easily taken 30 minutes if it wasn't for DNS. DNS ended up being the big bottleneck on the whole process, due to the time it takes to propagate. This is something we'll need to do differently, if we repeat this operation in the future.

In the end, the work was made a lot simpler thanks to the Agile Platform. Not only because it's totally prepared for these redundancy server scenarios, but also because it's so easy to change configurations and have everything running with the new settings in no-time.

Maybe even more important, the Agile Platform made it fast to split the components we wanted to keep in-house, and glue everything together with an SOA architecture. Being able to be <a href="http://www.outsystems.com/company/news/2010/outbynumbers-agile-platform-efficiency/">extremely fast</a> really opens a world of possibilities!

If you want to learn more about the cloud and how the Agile Platform can help you, click <a href="http://www.outsystems.com/cloud/">here to visit our cloud page</a>.

