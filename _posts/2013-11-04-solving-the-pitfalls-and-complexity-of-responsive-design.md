---
layout: post
title: Solving the Pitfalls and Inherent Complexity of Responsive Design
date: 2013-11-04 09:06
author: gveiga
comments: true
categories: [Dev Zone, mobile application, order management system, outsystems platform, responsive design]
---
A large enterprise customer recently challenged us to explore the viability of responsive design when building a mobile application for their sales team to use in the field.

It was an interesting request because it's not something we would have suggested. Our recommendation to clients had always been that application functionality should be based on use cases that make sense to the device. Responsive design, we argued, brings too much complexity and greater costs in maintenance and testing.

<!--more-->

However, when this customer explained that their existing mobile app suffered from low adoption rates and their agents preferred finding a way to use the full enterprise version online, we were determined to find a solution.
<p style="font-size: 16px; padding-top: 15px;"><strong>Could we figure out how to respond to different use cases with a single code base using responsive design?</strong></p>
People use devices and apps differently. We know this from field testing, from understanding user tasks, and from studying analytics. As it's unlikely that organizations are willing or able to implement and maintain the scale of investment needed to understand how each user is using their device particularly when several distinct user profiles are involved. This particular customer's need was to see if the OutSystems platform could break them out of the mobile application rat-race the same way it had helped them with desktop applications.

What we understood from our experience at other customers was that users get frustrated when they cannot perform the same actions in the mobile application that they can in the desktop version.

It took time and tinkering, but our "a-ha!" moment came when we discovered that the OutSystems Platform could create a set of content placeholders that implement and contain the required responsive design.

&nbsp;

<a href="https://www.outsystems.com/blog/wp-content/uploads/2013/11/order-management-thumb-600x446-5221.jpg"><img class="mt-image-center" style="text-align: center; display: block; margin: 0 auto 20px;" src="https://www.outsystems.com/blog/wp-content/uploads/2013/11/order-management-thumb-600x446-5221.jpg" alt="order-management.jpg" width="600" height="446" /></a>

We accomplished this by creating building blocks for more than business UI. By centralizing all the inherent complexities in what we call an eSpace, and by creating web blocks for specific UI patterns - with their own stylesheets and javascript and logic - we created a framework with an enhanced page layout and with the intelligence to react to specific device constraints. Developers can now easily and quickly develop and migrate responsive web pages without worrying about the complexity behind the responsive behavior.

The benefit of these placeholders is that they avoid some of the maintenance pitfalls of responsive behavior, and when they don't, when there is a page that doesn't adapt as it should, the combination of the platform's device querying ability and rapid change capabilities means that a maintenance team can change or replace these pages with other solutions when required.
<p style="font-size: 16px; padding-top: 15px;"><strong>An Opportunity</strong></p>
Approaching responsive design this way has a major advantage for users - the pages and patterns are the same from device to device. So if the user knows the web solution, he will recognize it in different devices. A few interactions - recovering the menu, for example - might change, but otherwise it's the same app.

Thanks to the massive automation of the OutSystems Platform, our customers are able to handle the complexities of responsive design by automatically fixing what would have broken the bank to do by hand.

In the end, we were able to create an experience that translated nicely from desktop to tablet to smartphone due to the way workflows were implemented and the adaptive ability of the layout, patterns and controls.

This pre-built web block approach shows the platform's great versatility and makes responsive design easy to use and maintain. In fact, I believe we can eventually create something like <a href="http://en.wikipedia.org/wiki/Twitter_Bootstrap">Twitter Bootstrap</a>, which will simplify UI development and create a smaller learning curve for developers. Developers could then create their own "Live Style Guides" and not need to learn hundreds of CSS classes required to implement responsive design. They would only need to learn about a few web blocks and drag-and-drop them into their interfaces.

You can't avoid a pitfall any easier than that.

Have you had a responsive design nightmare that could have been avoided with automation and a component like a "Live Style Guide"?
