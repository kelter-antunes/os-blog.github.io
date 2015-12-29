---
layout: post
title: High Performance Web Applications
date: 2010-04-16 17:51
author: cga
comments: true
categories: [code generator, code optimizer, database connection pooling, Dev Zone, memory optimization, performance management, viewstate]
---
<div>
<div style="margin: 6px; padding: 0px; font-family: Arial; font-size: 10pt; counter-reset: __goog_page__ 0; line-height: normal;">

António Melo of OutSystems, started his session on web applications performance by setting the scene about the several performance concerns that need to be taken into consideration: 1) define quantitative targets; 2) estimate the infrastructure required to go live and 3) evaluate performance and scalability as you move forward.

Moving forward with his presentation, António listed a few issues to consider at each of those stages. One is the data transfer between the browser and the server. <!--more-->Cache is good, but you shouldn't rely too much on it. Browsers will discard it every so often due to their size. Other issue is the dynamic content or so called "viewstate" of applications, which can get really big if you don't care about it. António shown how the Agile Platform does the automated optimization at the code generation level without having to have developer to understand how does advanced web application session management works and think about it on a case by case basis.

António explained how the OutSystems' Agile Platform takes advantage of Service Studio models to identify dependencies between business rules, User Interface and database to optimize a series of items in each running application. If a specific database record or column is not going to be used, why leave it there? The Platform takes care of eliminating waste in runtime!

Using the Agile Platform's Service Center, António showed how to track down any outstanding performance issues that haven't been optimized by the built-in code optimizer, automatically getting analytical information about performance of the application out-of-the-box. Pretty cool!

Additionally, he described how the Platform uses server-side cache, asynchronous logging, log rotation and scheduler throttling to improve performance. He listed several other optimizations done by the Platform, such as database connection pooling, dataset late loading, horizontal scalability, automated indexing and more. All automated by the Agile Platform.

Finally, António presented the audience with some additional real world numbers. One of OutSystems customers was getting 1,100,000 page views per day with 3 servers, increasing to 1,900,000 pages views in only 6 months.

In a nutshell: according to António, before development you shall define your targets and performance requirements. During development you shall include those requirements as you do with business requirements and keep measuring and improving, the agile way! After going live don't forget to keep monitoring performance and act accordingly.

Lessons learned: even if using built-in optimizers, such as those provided by the Agile Platform, please consider performance requirements at the same level you consider business requirements. You don't want performance to impact your ability to do business.

Want to learn more? Go to the Agile Network and find <a href="http://www.outsystems.com/NetworkSearch/Entry_Search.aspx?SearchQuery=performance">more about performance</a> with the Agile Platform.

</div>
</div>
&nbsp;
