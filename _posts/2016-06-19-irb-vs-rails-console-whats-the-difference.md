---
layout: post
title: "irb vs rails console? what's the difference"
tags: [ruby, rails, software development]
---
{% include JB/setup %}

Every ruby/rails programmer knows how much valuable are friends like
**`irb`** and **`rails console`**. I particularly am very fond of them, because
any time I want to try something, I instantly use them. You also must be
aware of **`bundle console`** and **`bundle exec irb`**.

So, actually we have four such tools, but what is the difference between
all four of them, if any.

###irb vs bundle exec irb vs bundle console vs rails console

####irb
**`irb`** is just plain simple ruby console. What I mean by that is it just
loads your core ruby libraries. It does not care whether you have
gemfile lying around. So if you want to add anything else, you would
need to use **`require`**.

If you have a gem installed, you can require that gem inside irb. If you
used **`bundler install`**, irb may not necessarily require the same version
of that gem, since it ignores your gemfile and thus gemfile.lock as
well.

####bundle exec irb
**`bundle exec irb`** comes to help, when you want to require the version of
gem specified in your gemfile, something that irb cannot. **`bundle exec
irb`** allows you to load the gems that your bundler knows about and only
the gems that bundler knows about.

####bundle console
**`bundle console`** goes one step further **`bundle exec irb`**. The latter
allows you to load gems specified in gemfile, but the former already
requires them for you

*Tip - you can require all the gems in **`bundle exec irb`** if you do
**`Bundler.require`** inside the console. All the gems will be required,
except for those which aren't marked **`required: false`***

####rails console
`rails console` manages to jump one step ahead of `bundle console` by
even loading the environment for you. So inside its console, you can
play around with your rails app and your database connections work and
everything works the way you would expect. Its a real life saver, trust
me on that. This is most helpful when you are working on a rails app.

*Tip 2 - if you do **`require_relative config/environment.rb`** inside the
console of `bundle console`, you would get the equivalent of **`rails
console`***
