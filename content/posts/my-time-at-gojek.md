---
title: "My Time at Gojek [work in progress]"
date: 2020-08-29T20:12:13+05:30
draft: false
toc: false
images:
tags:
  - untagged
---

> I need to be the dumbest guy in the room

this is what I told myself when I set out from college and began my career.
I wanted to be at a place where I am surrounded by smart people, brilliant at their job, willing to learn and willing to teach.

Fortunately, an internship at Codeignition in the summer of 2014 gave me exactly that. I found people with proven credentials and wanting to stretch themselves even further, who not only expect nothing less from themselves but also from the people around them.

Shortly after, I moved to Bangalore where Codeignition would work along with C42 for Gojek. Gojek had launched their mobile app in 2015 but their servers were unable to keep up with the demand. With Sequoia playing the matchmaker role, Gojek became our client and we started consulting for them.

Inside a residential building in Bangalore, a cohesive unit of 30 people started working on Gojek. We all used to have one single standup. After a few months, Gojek acquired us.

I did not completely understand what would that mean for myself on a day to day basis. We were pretty small firms at the time, and I know my founders had always been worried to get enough clients so that they can give out our salaries. I thought maybe they and us will have a easier life now. oh boy, I could not have been more wrong.

What happened next was a roller coaster of a ride, with its fair share of ups and downs. It has been completely fascinating, humbling and full of learning to say the least.

---

## Go-Kilat: my first product

With goals of learning how software is written and shipped in companies, I began working on a product called Go-Kilat. Kilat is bahasa for lightning (bahasa is the official language of Indonesia). Consumers would be able to order stuff online and get deliveries within few hours rather than having to wait for multiple days.

I had studied software engineering previously in my college but never really had a feel for it. Primarily because when I used to write code at that time, I was the only one who was working on it, and defining what I wanted the code to do.

But now it was different, there were people defining what we need to build, and multiple developers working on it at the same time. Also requirements kept changing. So we needed to be agile enough to incorporate those changes and wrote our code in a way that could make those changes possible.

I got to pair with some amazing developers during this project. Pairing with people better than me allowed me to see how they think of the problem, the solution and how they went about executing the solution. I felt that my rate of learning improved significantly. Interacting with them also clarified my own thoughts and forced me to pickup new ones.

Once code for a story was written, we raised PRs. I got critical feedback all the time, and I cannot be thankful enough to the people around me at the time who put it in significant effort to go through my PR. Even indentation mistakes were pointed out. I always felt that I leveled up as a dev, once I worked through comments on my PR.

But it was not just coding, we had to ship our product too. Being the product engineers that we were, it meant the onus is on us to make sure we ship it. I got firsthand experience in setting up different environments to test out our product. I was always fascinated whenever I got my hands on infra and I took great pride in that.

I still remember the day when we took GoKilat live, everything went smooth. The first order came in shortly, and our product manager personally called the first consumer of our app and thanked her for using the product and asked for feedback and pain points while using the product.

Seeing people actually using something that I built, was a euphoric moments. I had tasted something and I wanted even more of it now.

---

## Allocation: how high can you go

The goal of this newly setup team is simple - to achieve 90% booking conversion rate. This statement was part of email written by our then CEO Nadiem Makarim when allocation team was incepted within Gojek. 

This is where I got truly excited about my work. There were engineering problems to solve but the domain itself was fascinating to say the least. We had different products which had their own booking state machines, but all getting fulfilled by the same driver supply.

At the time, Gojek was doing around 400k bookings completed max on a good day. As part of this team, that number rapidly started growing. I remember whenever I had to take a break from my usual work, I would just open up the business dashboard and start looking at what is going on. A lot of the team members and stakeholders used to be on a call every friday night, seeing the booking completed numbers go up. That was a dream moment for me. I remember when I watched the movie The Social Network and in it was this one scene where all employees of facebook stare at this big screen of total user signups and the number reaches like a million or billion. From that moment, I wanted to experience that feeling. Little did I know that I will get to experience it at such an early stage in my career.

Within one year, we managed to do 1 million completed bookings daily with booking conversion rate just below 80%.

My skin in the game increased when I was made tech lead for the surge project. At that time, gojek bookings never charged a surge fee like uber. Simply because we were always in developer crunch. 

I remember there were 6 items that were crucial because of investor expectations and 2 of them had come to our team. One was surge, other was route based allocation. Route based allocation was done by my friend Sartaj while I was made incharge of surge pricing.

A team of 6 set out to achieve this goal. This was also a very unique problem in surge pricing because of the nature of gojek products and services. All products except for Go-car, had the same supply pool. Thankfully, we had a bunch of smart people who were able to come up with a genius solution to this unique problem. We aligned and got into implementation.

I still remember when we launched surge pricing for bikes, people inside the org went crazy. It was tough for them to get a gojek when they left office, because of the rush hour. Now, they were getting drivers in a matter of seconds. I felt so proud of myself at that moment. This is exactly why I work, to create value and to make lives of people around me a little bit easier.

By the time I left the team which is about 1.5 years, Gojek was doing close to 2 million completed orders daily with a booking conversion rate above 80%.

---

## Atlas

> It doesn't make sense to hire smart people and tell them what to do; we hire smart people so they can tell us what to do - Steve Jobs

Since I considered myself smart, I expected myself to have an opinion of what is the problem that needs to be solved, crisply defining that problem statement for others to understand and come up with a solution to get started solving it.

Atlas was a new beginning for me in many sense. I started working with an entirely new set of people on very different problem statement. This was my first time working in an internal platform team amd challenges were very different to what I had experienced previously.

The first thing I experienced were consensus/alignment problems. In the past, I had just taken it for granted but now I was facing challenges to bring everyone on the same page. 

I was incharge of solving uptime tracking problem for gojek services and while we were able to build a product for the same, getting it adopted internally was a different problem altogether. I made some classic product mistakes and did not voice out my opinions at a couple of occasions, not my proudest moments overall.

Soon uptime tracking became this huge problem statement. I will try to explain. Basically at the time, microservices were getting invented left right and center. There was no standardisation and there was zero visibility for people higher up the ladder. How do I bring that visibility? What is it that I should be building that benefits the entire Gojek org and allows us to scale efficiently. I was very naive of an engineer at that time to even realise what am I getting into. I was not able to communicate to my team what are we trying to solve because neither I nor my stakeholders had an idea of what needed to be done. I took it as a failure of myself and could never stop thinking on what exactly is the problem statement. Even after I changed teams and switched to a different problem statement, I could not stop thinking about it. I had experienced failure first time in my professional career and I wanted to rectify it. This is not done, we will get back to this later.

---

## Singapore Launch

Uber had exited the Singapore region which led Gojek to launch its product in a first world country. Everything happened so quickly. I remember discussing Uber's exit, then discussing that Gojek may enter the market and then deciding on the team which will work on this project. It all happened in 2 weeks. I just love this kind of speed on decision making.

A team of 6 developers, 1 QA, 1 PM and 2 designers set out for this initiative. This meant frequent travels to Singapore office. I personally had a blast, getting to live in another country for so long. I was able to converse in English with the users and I could feel when the launch was edging closer as to how exciting it is.

This was different from working on one or two codebases. Our work now spanned across every bit of the architecture that was essential in serving a booking request on our transport app. Scoping it all out, communicating dates so that every other business team can align with their activities like driver onboarding, marketing etc in parallel with the product launch.

This was the kind of thrilling work which I strive and thrive on and the reason why everyone should work in startups, atleast once in their lifetime.

---

## Kernel - unfinished business

> to hell with circumstances I create opportunities - Bruce Lee


I joined Kernel because I had unfinished business in Gojek. My previous stint in an internal platform team was not great, the product that I owned at the time was not adopted within the org and soon found its place in the graveyard. That had bothered with me for a long duration because I realised that I am not able to think about engineering at bird's eye level. I contiously was assessing what I did wrong, what is currently ongoing in the org which needs to be fixed. I had spent so much time thinking about the infra platform that I just had to get my hands dirty one more time.

I started as a lead on the newly formed analytics team within kernel at the time, because I thought a lot about why our internal platforms team fail and the current problems within the state of engineering org at Gojek. There were no insights about our product engineering teams and services. I was (still am) a strong believer that analytics is something on top of which our engineering strategy and governance can be defined.

Kernel took over as the core infrastructure team of Gojek in January of 2019. The idea was to build infrastructure of Gojek as a product and not simply run it as operations. It had one mission statement - *to make product developers productive*

Gojek had scaled rapidly in the past few years where team sizes have grown 10x, our core infra platform was lagging behind. We were soon entering 2020 but with 2015 tech. People on the team were swamped with tickets and putting out fires all day. And were experiencing an existential crisis because they had lost track of what are they building that will eventually make the Gojek world a better place. While their fellow colleagues in product teams were shipping features that had a business impact with quantitative insights, folks here had no idea of what is the problem that they are solving.

We started with deriving data for a bunch of queries and soon we realised that it takes a lot of time to derive data. Why? information was scattered across sources. Only people with tribal knowledge could have worked in my team at the time. One google cloud project that had been live since the beginning of the time was called Gojek's history of infra museum. It was clear that before we even started with analytics, we had to fix the information fragmentation.

Fixing the information fragmentation would help us in solving
- ownership problems (who owns this?)
- one source of truth for different entities (how many services are live?)
- domain of the problem on which teams can be structured with clear boundaries

We called this knowledge graph and began executing on this strategy.

Coming to this point was not easy at all. The team suffered from lack of delivery, clarity of the problem and negativity was starting to creep in. I saw this as an oppurtunity to come up with my own ideas, sell them within the team and get them implemented. I myself had no clarity on the problem but I believed there was a problem worth solving and I knew that to make Gojek a truly great engineering company and be part of something like FAANG, the foundational infra and platform needs to be amazing. Simply based on this belief, I woke up and went to work everyday and I believed in my thought process that soon I would figure out problem statement in a way which I will be able to communicate to other folks across the org.



- knowledge graph as strategy for infra as a product
- building delivery rhythm
- scaling my managerial self