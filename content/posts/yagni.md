---
title: "Basic Principles of software design: Yagni"
description: "You ain't gonna need it"
date: 2015-06-12T01:53:00+05:30
draft: false
toc: false
images:
tags: 
  - yagni
  - software design
---

Welcome to third and final part of the series "Basic Principles of
software design". In this part, we will be knowing about YAGNI, yet
another simple but realistic and powerful concept.

You aren't gonna need it or YAGNI in short states that a new feature in
a code should not be added, unless and untill it is absolutely
necessary. It seriously discourages the practices of adding features
that are not necessary at that present point of time, but the programmer
thinks it might be useful in future. YAGNI states that coding such
features for the future is not necessary at all, instead it focuses on
improving the current features.

YAGNI in principal belongs to extreme programming. It is meant to be
used to several other practices such as continous referencing.

YAGNI has following benefits :

-adding new feauture will extract time from testing and improving the
current features, since the new feature must be debugged, documented and
supported

-that new feature might constraint the programmer for the future
development of the code, which is certainly not good

-such new features are difficult to fully define, which makes it hard to
code and test. So even if that feature turns out to be necessary for the
future, you have wasted your time previously and refactoring might not
be that easy anymore

-Defy YAGNI and there is a high probablity that your desired software
might turn into a bloatware. ( see here - http://www.webopedia.com/TERM/B/bloatware.html)

So you might be thinking now, what is bad about adding new features.
What if these features might be needed in the future. Yes, you are right
and this is a good question, even I thought about it too. But remember
the agile practices will give you the time, to add these features in the
future. As it is an iterative process, you need not worry about the
future, just focus on the present. Read Martin Fowler's blog post, for a
detailed information. ( http://martinfowler.com/bliki/Yagni.html )

Keeping your code ready for unexpected changes is about simple design.
Adding extra features beyond necessity always will make the design
complex. Remember KISS.

Concentrate on what is schedueled for today.
