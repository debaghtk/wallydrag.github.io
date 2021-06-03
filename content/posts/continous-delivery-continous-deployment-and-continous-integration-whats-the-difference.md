---
title: "Continuous Delivery Continuous Deployment and Continuous Integration Whats the Difference"
date: 2015-11-29T01:53:52+05:30
draft: false
toc: false
images:
tags: 
  - CI, CD
  - continuous integration
  - continuous delivery
  - continuous deployment
  - devops
  - culture
---

Continuous delivery, continuous deployment and continuous integration
are three words that you might be hearing regularly these days. I was
initially confused as they seemed pretty similar to me and I bet half of
the crowd are confused too. So I put on my superhero mask and googled
the three :D

Turns out, these three, while being really similar and related to each
other as well, have pretty subtle differences.

Continuous integration is when say, a group of developers are working on
a project. The rule of thumb is, you write a patch of code, you push it
on the repo and the continuous integration software, whatever it may be,
tells you whether that code is working correctly or not. It does so, by
running automated builds on it. If the code is not right, the rest of the
team is notified that they do not push their code right now, untill the
bug is sorted out. CI requires you to write code in small amount and
make atleast 2-3 commits daily. This approach leads significantly
reduced integration problems and allows software to be made at a rapid
speed. Since, everyone's code is integrated frequently, software
deployment becomes less of a hassle. This is the first step in achieving
a production-ready software as soon as the developers write some code.

You just can't achieve continuous delivery and continuous deployment
with continuous integration.

Continuous delivery and continuous deployment have far more in common.
And there is only one difference.

Continuous deployment is when a change in code, is integrated and
deployed continuously. So your continuous integration pipeline, when it
runs after a commit and say the patch is right, it will be deployed
automatically.

Continuous delivery is exactly like continuous deployment, except for
the the deployment is manual. The code at any time is production ready,
so whenever your client demands the changes in code be deployed as soon
as possible, you are always ready. You become superman for your client. 

![Continuous Delivery vs Continuous Deployment](/images/cont.jpg)\
image credits: [Crisp's blog](http://blog.crisp.se/2013/02/05/yassalsundman/continuous-delivery-vs-continuous-deployment)


I hope this blog is informative enough to point those differences. I am
attaching some links for further, if you just have some time to kill. 

- [Martin Fowler's post on Continuous Delivery](http://martinfowler.com/bliki/ContinuousDelivery.html)
- [Martin Fowler's post on Continuous Integration](http://www.martinfowler.com/articles/continuousIntegration.html)
