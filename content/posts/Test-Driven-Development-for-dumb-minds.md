---
title: "Test Driven Development for Dumb Minds"
description: "TDD is very underrated. Everyone should write code in this manner, everyone"
date: 2015-05-26T01:46:31+05:30
draft: false
toc: false
images:
tags: 
  - tdd
  - test driven development
---
The following blog post discusses Test Driven Development and aims for
people who want to understand what it is, can get a fair bit of idea
after reading the post.

No, I am not going to begin with a story here. Let's not waste any more
time and dive straight into the world of Test Driven Development.

## What is Test Driven Development?

You might have heard of the above term in your college course *software
engineering.* If you are still in college, chances are you don't know
exactly how it is implemented in a code.

Let's just say, TDD wants to you to write a test, before you write a
small patch of code. That way, you make sure that very certain small
patch of code performs its intended functionality. We will understand
this in a bit more depth later.

#### So, what the heck is testing?

Suppose you wrote a program, that takes two numbers as input, and
outputs the sum of those numbers. You compile the code, and if it has no
errors, it would run without any problem. Then you would give two
numbers, to see if the code gives the desired result. The last step you
did was testing the code. To see whether your code is working desirably
or not is testing.

#### So, what is so cool about TDD?

The process of testing that we applied on the above case has certain
pitfalls

- You had to write the entire program, before you can test. Imagine
writing thousand of lines of code for a program, but with the
uncertainity that whatever you written may not be correct.

- Once you have written your big program, it would be hard for you to
debug if a error occurs or your program doesn't run properly. This way
of testing won't pinpoint that specific segment of code, which is
causing the program to fail.

- The way of testing is manual, and you do know that automating things
are cool. Hey, that's the reason we code, right. You can check for
numerous cases when you have written a test, but I know that you won't
check for numerous cases when you would have to feed the input
every time. Yeah, humans are lazy.

- Take one example, suppose you maintain a somewhat large codebase on
github and people constantly send you pull requests. Since you haven't
written any test, you will need to run your program, with each pull
request, see whether it is working or not. And you still won't be sure
whether that patch of code is absolutely correct or not.

Now, if you would have followed the TDD paradigm, things would have been
different and life would be much simpler, let's see how :

- The unit tests will provide constant feedback that each component is
still working. You don't need to write the full program to check your
code. TDD will give you the power, to run every unit of individually.
That way, you can be sure that whatever you have coded till, is correct.

- Debugging becomes a lot easier. Running the tests will pinpoint that
part which is causing the program to fail, if any. You don't even need
to compile and run the program itself, just run the tests.

- You can put numerous test cases to check the code. Automating things
will make the work faster but rigourous checking will also be ensured.

- You don't need to understand everyone's patch in your code. Just run
the tests, if the patches are good enough, the tests will run fine and
you will know which patches to select for your code.

#### Hmm, but how do I do it?

The process of TDD is best understood by cycle called **Red, Green and
Refactor**, shortly known as RGR.

Just read on to know what RGR means exactly:

-Understand the requirements of the story, work item, or feature that
you are working on.

-Red: Create a test and make it fail.Imagine how the new code should be
called and write the test as if the code already existed. Run the test.
It should fail. This is a calibration measure to ensure that your test
is calling the correct code and that the code is not working by accident.
This is a meaningful failure, and you expect it to fail.

-Green: Make the test pass. Write the production code to make the test pass.
If you've written the code so that the test passes as intended, you have
done you job. If new functionality is still needed, then another test is
needed. Make this one test pass and continue. When the test passes, you might
want to run all tests up to this point to build confidence that everything
else is still working.

-Refactor: Change the code to improve the design while ensuring that all
tests still pass.

Repeat the cycle 2-3-4. Each cycle should be very short.

## Conclusion

No fairy tale ending here. Just go out and get your hands' dirty with
TDD. Only practicing to write code by TDD guidelines will make you
understand its concepts better. Run away fella, run away now.
