---
layout: post
title: "Basic Principles of software design part 2- KISS"
description: ""
category: [KISS, software design]
tags: []
---
{% include JB/setup %}

This is the second post in the series of "Basic principles of software
design". In part 1, we discussed about DRY. Today, we will be knowing
about KISS. Yes, you read it right.

KISS is acronym for 'Keep it simple stupid'. This principle, as simple
as it sounds, is not easy to implement. I personally find it correct in
so many aspects of life, for me KISS is very philosophical.

Moving onto the software part, every developer should try to write code
for a system, as simply as possible. Simplicity does not mean quick and
dirty. Simplicity should be achieved, keeping in mind the code is easy
to maintain and the end-product is intuitive to user. Complex systems
are hard for humans to manage. Therefore, simplicity is a primary
concern in software development.

This is not to say that features, even internal ones, should be
discarded in the name of simplicity. Indeed, the more elegant designs
are usually the more simple ones. It often takes a lot of thought and
work over multiple iterations to simplify.

For an example, Ruby has conventions among its developer community, such
as a class name should begin from a capital letter, eg. class Dog.
Variable in ruby are named in snake case, eg. power_of_input while
variable in js are named in camel case, eg. powerOfInput. These
conventions are widespread, and helps in spreading a general awareness,
such as a developer across the globe would be able to understand so much
of your code, without having to put too much of his thought process.

Such conventions should be followed, because if you are not, not only
you will be having a hard time, but your other fellow developers too.

KISS also comes in handy, when you are trying to over simplifying
things. That leads to unefficient code and new problems may arrive.
Chances are the problem you were set out to solve might not have been
solved. 

KISS also puts a boundary on applying other prinicples and guidelines
such as DRY and SOLID. If you have to unDRY certain parts of your code,
and if that way, it becomes simple, KISS will allow that. 

When in doubt, just remember this quote from ALbert Einstein: 'Things
should be made simple but not simpler.'
