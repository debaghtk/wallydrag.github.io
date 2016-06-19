---
layout: post
title: "Learning Git"
description: ""
category:
tags: []
---
{% include JB/setup %}

### So what is Git?

Git is a software that keeps track of changes that you make to files and
directories. It is especially good for text changes that you make.

Imagine you have a document. At that moment, it is on version 1. You
make some changes to it and save it. That would be version 2. You make
some more changes, you get version 3. Now, git will keep track of those
3 different versions for you and it allows you to move back and forth
between different versions, to compare the different versions and to see
the changes in each one. Since it is mananging these versions of the
document for you, it is genereally referred to as a version control
system (VCS).

All VCSs ever created were primarily for managing source code for
computer programmes.

### A brief history

*(you can skip this part)*

- Source Code Control System (1972, closed source, free with Unix) - It
isn't the first, but the first that was popular. Instead of saving each
version of the file, SCCS saves the first version i.e. the original
document and then it starts saving the snapshot, of what the changes
were. So, it won't save version as is, but will save the changes of
version 2 and version 1. Simiarly for version 3, it will save the
changes of version 3 and version 2. Now if you request for version 3, it
will take version 1 and put 2 sets of changes to it.

- Revision Control System (1982, open source) - this was a big upgrade
over SCCS as it was cross platform. Also, it had much more functionality
and was less hassle free than SCCS. It was fast too. Unlike SCCS, it
saved the most recent version of the file and applied changes to revert
back to previous versions. Much of the speed came from this change,
since people do much more work on current file.

- Concurrent Versions System (1986, open source) - A problem with SCCS
and RCS was they only allowed to work with a single file, but not in
sets of files. Not only CVS solved it, it brought the idea of restoring
our code, called code repository and put that on a remote server and
more than one user can work on these files at the same time.

- Apache Subversion (2000, open source) - The idea of working with
remote repository was further improved upon by SVN, it was faster than
CVS and allowed saving non-text files like images. It watched the
directory as a whole while CVS watched the directory as a group of
individually named files. Adding, removing, renaming files gave CVS as
hard time but SVN did that with ease. SVN does a transactional commit
and apply all of the changes to directory or none at all.

- BitKeeper SCM (2000, closed source, proprietary) - It had the feature
of distributed version control. It had a "community version" was free and it was used for the source code of the Linux Kernel. In April 2005, the community version stopped being free. And this was the beginning of Git.

- Git - created by the Linus Torvalds. Git was replacement for the
BitKeeper to manage Linux Kernel source code. It has following features:

  - distributed version control
  - open source and free software
  - compatible with Unix like systems (Linux, Mac OS X, and Solaris),
  even windows
  - faster than other source code management systems
  - better safeguards against data corruption

### Wait, what is distributed version control?

This is an important feature of git. VCSs of the past like SVN, RCS use
a central code repository model that is that there is one central place
where you store the master copy of your code and when you're working
with the code you check out a copy from the master repo. You work with
it make your changes, and then you submit those changes back to the
central repo. Other users can also work from that repo submitting their
changes. And it is upto as users to keep up to date with whatever is
happening in that central code repo, to make sure that we pull down and
update any changes that other people have made.

Git doesn't work that way. Git is distributed version control.

- different users (or teams of users) maintain their own repositories, instead of working from a central repo.

- changes are stored as "change sets" or "patches"
