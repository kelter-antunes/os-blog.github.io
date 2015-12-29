---
layout: post
title: Developer Diary: Justin James gathers user feedback with ECT
date: 2010-07-06 16:58
author: Rodrigo
comments: true
categories: [Agile Platform, Application Development, Dev Zone, ECT, Justin James Developer Diary, Tech Republic]
---
With <a href="https://www.outsystems.com/blog/aboutagility/2010/06/jjdiary-application-integration-and-deployment.html">Rat Catcher deployed in public Beta</a>, it was now time for <a href="http://techrepublic.com.com/5213-6257-0.html?id=2926438&amp;tag=workspaceTop;wsBannerLeftCol">Justin James</a> to start gathering user feedback on his application. To do this, Justin installed and configured OutSystems' Embedded Change Technology (ECT.) You can read about his experience in his <a href="http://blogs.techrepublic.com.com/programming-and-development/?p=2772">latest diary entry</a> in <a href="http://techrepublic.com.com/">Tech Republic</a>.
<div><!--more--></div>
<img class="mt-image-right" style="float: right; margin: 0pt 0pt 20px 20px;" src="https://www.outsystems.com/blog/wp-content/uploads/2010/07/etc_button2.png" alt="etc_button.png" width="173" height="50" />
<div>"ECT is a technology that allows the end users of my application to place a pinpoint on the working application, type a text message, and hit a button to submit their feedback. In the back-office, I then receive the screenshot of the application web page with the user's pinpoint plus the text message. (You can see a <a href="http://www.outsystems.com/platform/#capture-contextual-feedback" target="_blank">quick demo of the ECT</a> in action.)"</div>
<div></div>
<div>
<div style="padding-top: 20px;"><b>Getting everything ready for ECT</b></div>
</div>
<div></div>
<div>ECT makes use of Enterprise Manager, a solution provided by OutSystems that centralizes all common administration tasks such as users, roles and the existing applications' back-offices. Installing it is easy. Just <a href="http://www.outsystems.com/NetworkSolutions/ProjectDetail.aspx?ProjectId=64">download it from the OutSystems Network</a> and use the Solution Pack Tool to 1-Click publish the solution. "Next, you repeat this process, but with the ECT solution; <a href="http://www.outsystems.com/NetworkSolutions/ProjectDetail.aspx?ProjectId=7">download ECT here</a>, open it, and click 1-Click Publish."</div>
<div></div>
<div style="padding-top: 20px;"><b>Configuring ECT</b></div>
<div></div>
<div>Justin provides a great step-by-step explanation in his article on how to configure ECT in Enterprise Manager, and moves on to using the ECT configuration wizard to customize its behavior. "The wizard is pretty self-explanatory from here. One thing to keep in mind is that you may not want to add ECT to every eSpace on a production server. Then again, you might want to after all!"</div>
<div></div>
<div style="padding-top: 20px;"><b>Collecting feedback</b></div>
<div></div>
<div>With ECT up and running, users started to send feedback about RatCatcher. As Justin puts it, this "feedback system is far better than receiving the typical email from a user where they have a hard time describing what the problem is. It can be used for bug reports as well as suggestions for improvements."</div>
<div></div>
<div>
<div>"While this is the type of feedback that could be given through email or a trouble ticket, ECT's ability to show me exactly where on the screen the user had a problem is extremely useful. In addition, it functions as a simple issue management system."</div>
</div>
<div></div>
<div>One point Justin mentions is that he might have "to find a way to educate users about ECT". ECT is very discreet and "the bottom right is the least viewed part of the screen." This was actually a design decision we made at OutSystems. Although we want ECT to be ever-present, so users can submit feedback whenever they want, we don't want it to get in the way of the application.</div>
<div></div>
<div>I hope Justin keeps getting excellent feedback from his users on RatCatcher, and I'm sure the app will continue to get better and better! In the meantime, we'll be waiting for the next installment of the Developer Diary!</div>
<div></div>
&nbsp;
