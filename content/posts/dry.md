---
title: "Basic principles of software design: Dry"
date: 2015-06-04T01:50:29+05:30
draft: false
toc: false
images:
tags: 
  - dry
  - software design
  - don't repeat yourself
---

I am thinking of doing a series of blog posts this time, that
underlines the importance of some of the very basic principles of
software development. I personally felt that a programmer should be
introduced to these principles as early as possible. These fundamentals
may seem easy on the eye, but it takes a while to implement them
in your code.

Imagine a situation. Suppose you have a dog at your house, that needs
milk every morning. You can't buy milk in bulk because storage is a problem.
So, you can either go to the milk shop daily in the morning and buy milk, or
you can go just once and pay him for a subscription so he will send someone
to your place to deliver the milk. So which sounds best to you, decide for
yourself. *A good programmer for the second one*

This is the first part of this series of blog posts and today, we are going
to know about a software engineering principle called **DRY** - short form
for *Don't Repeat Yourself*

This principle came up in the book *The Pragmatic Programmer*, by
Andy Hunt and Dave Thomas, but the concept, itself, has been known
for a long time. One can understand the idea of the principle by just
looking at it. And it's pretty relevant not just in programming but I
believe in many aspects of life.

So, how do we work on a complex problem that we know requires effort in
writing code? An evergreen solution is to breakdown the problem into
several small components, where each performs some specific functionality.
Then these components together will be the solution to the original
problem. Large software projects can be overwhelming, but dividing them
into parts makes it easier for us humans to understand them.

For example, if we're building a content management system, the part that
is responsible for user management will be a component. This component can
be divided into further subcomponents, like role management, and it may
communicate with other components, such as the security component.

As we divide systems into components, and, further, components into
subcomponents, we will arrive at a level, where the complexity is reduced
to a single responsibility. These responsibilities can be implemented in a
class (we assume that we're building an object-oriented application).
Classes contain methods and properties. Methods and subparts of these
methods are calculating or containing the smallest pieces that build your
logic.

*The DRY principle states that these small pieces of logic may only
occur exactly once in our entire system.*

DRY is a philosophy that packages logic into representations.
There are many ways of achieving DRYness. Hunt and Thomas suggested
(among other things) code generators and data transforming. But,
essentially, DRY is a philosophy that packages logic into representations.
And each logic must have a single, unambigous representation in your code.

Sounds easy, right? Well, that's not usually the case. DRY and modular
architecture require good planning. To achieve a representational hierachy
from bottom-up, divide your application in a hierarchy of logically separated
smaller parts and let them communicate with each other. If you have to manage
larger projects, organizing them into components and using DRY within the
components is a good idea.

And while you write code, be lazy!!
