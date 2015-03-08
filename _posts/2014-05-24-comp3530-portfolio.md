---
layout: post
title: "Systems Engineering Essay"
date: 2014-05-24
---

This was originally posted on my old Google website for my COMP3530 course at ANU.  I've reposted it here for posteriority.

# Intro - What I want to achieve

Hopefully I will begin to understand a bit more about Systems Engineering as applied to programming and the software development process.  I'm already drawing a few links between concepts briefly named in Shayne's intro spiel and concepts that I teach as a PAL mentor for first years!  These range from thinking about why things are done in specific ways, where to expand and find knowledge, to identifying the underlying root causes of problems and acting on those rather than the symptoms, to finding possible pitfalls and mitigating them early on to avoid doing more work later.

I will have to wait and see whether any of these links I'm drawing right now between COMP3530 and other areas in my life will continue to be there throughout the course.  I certainly hope these links and others will help me form a "big picture" view of the similarities between the development and learning processes, and how concepts from one can be used interchangeably with the other.

Stephen Ellis's presentation was quite informative.  It certainly highlighted that when working with something so complex there is no way to accurately design it and control every aspect of the system.  I've certainly experienced this when conducting my research last year, where even though I had a working plan and a good idea of where I wanted to take it, the final solution seemed to grow more from pitfalls and last minute changes I had to work around than from the plan itself.  There was no way I as one person could know every detail of the interaction between project components, and I can see how this can scale to a design team working on an entire system.

**Tell us about another system failure blamed on software, but in which other 'system' issues were contributing factors?**

Whilst the current drama around it will have to play out in order to conclusively know what happened, the Obamacare website is a current system that I think highlights some of the problems I feel could go wrong when designing a system.  Even in its current state, it appears not to be able to handle as many requests per second as originally designed, nor does it rate insurance policies properly.

There are multiple reasons that such a system didn't hold up to the standards it was set -- however, the one that stands out the most for me is the fact that it had a centralised planning authority that designed the requirements and the system as a whole.  Because of this, the only way they could execute their design was to ensure coordinated action from a collection of entities that had no relation to one another, didn't know what was going on and had many conflicting end goals of the system.  Since the boundaries between areas were never thought through, these entities also did not know everyone else who was involved in the system, and as such had no ability to understand the system and give their input on it.

Because the design was centrally controlled, the planning team had to collect and process all the information themselves.  This led to a lot of information being dropped from information overload, and as a result of this the interfaces between parts of the system tended to fail, if not were unimplemented/unthought of in the first place.  An example of this is the display and rating of insurance policies based on the user's needs -- the system interface between the needs of the customer and the various policies was not thought out fully, and the system displayed policies that were completely unrelated, or failed to show that a policy had been rated at all.

Some of the system specifications that have people pointing fingers at the software had nothing to do with it in the first place.  One such requirement is that the system mandates that the country as a whole will get more medical care -- something that is entirely outside its scope of control!  In order for this to happen, there has to be more doctors, nurses and other medical personnel, which is something that the Obamacare system does not create or have any authority over.

# Systems Thinking

What we saw is a very simple way to deal with complexity, but I think that it is a skill to be able to simplify a complex system to a high level view that accurately reflects on everything that is going on.

In the end though, the fact that there are two ways of thinking about feedback in complex systems helps simplify the task a bit.  Keeping in mind the the concepts of both positive and negative feedback loops when analysing what's happening in a system could help us work out the root cause of a problem (which may lie outside the system as well) and enable the design of the solution to focus directly on the issues at hand instead of reacting to possible symptoms that may not be related at all.

I think that the "fixes that fail" template put forward by Newell and Proust gives a clearer picture to fill out what's really going on than just considering the problem and problem symptoms as the same thing (like in Senge's template), however I'm still unsure that there is not another area covering the extent of "fixes" targeting unrelated symptoms that affect other areas outside of the system.  Having a feedback template is also only a very high level view that can direct further inquests into what's going on but does not help solve the actual problem that is underneath and growing.  I suppose that such a solution would be specific and subject to the constraints enforced on the system by design or by outside entities.

Given such a diverse area as systems engineering, thinking about systems as simple loops and high level "movements" in a sense may help me understand and consolidate the many different areas involved in understanding it.  I think that trying to worry about every little detail at once will get overwhelming, and using systems thinking to ignore the details and focus on the core message will help me build up the jigsaw of systems engineering and how it goes together.  Certainly, applying this to areas such as sustainability and the engineering context of systems engineering will help reduce the huge amount of information to make it more manageable on a large scale, before exploring the finer details of each part to build up my own understanding of them.

As for a problem where I've employed systems thinking -- I suppose that one such example could be thinking about how students learn content and the thinking processes that they use to go from not knowing anything about a topic to fully understanding it, and everything else in between.  Implicitly I was thinking about the feedback loops in use that could modify the way they learnt, and how to tweak them so that we could leverage the feedback system to help students integrate knowledge from their first year courses in PAL.  We didn't focus on the details of the way each student went about their learning but instead tried to focus on what was similar to each student, and tried to derive a pattern that everyone seemed to follow.  We eventually found the key "landmarks" underlying the learning that showed where students were up to in their understanding, and from this we could address the needs of different groups and help them improve in a far more efficient way than before, where we were only reacting to what the students seemed to be missing at the time.

# The Engineering Context

The context of an engineer's role in a system is something I haven't really thought about before.  I guess that working on a complex system means that the responsibility placed on you to ensure your component works as designed increases as the system involves and/or impacts more people in the world.  Being an engineer means to me the purpose of designing and constructing a component so that it works as required, and no less (not sure about adding "no more" -- having something that is over-engineered could be seen as a positive in many industries, unless talking financially)

While I cannot give an example of when I was questioned from an ethical perspective on something I was doing as part of a larger team, I can imagine that this should play a large part in knowing why you are doing something as an engineer.  Indeed, to really do well in something it's likely that the "why" of doing something is just as important as the "how", since otherwise there is no purpose to doing it in the first place!  I suppose that knowing whether a system or item you are working on could be used against groups of people can be rather alarming.  However as Geoff pointed out in the week 3 panel, such a system can also save a lot of lives by eliminating groups of people plotting to kill other larger groups.  It all goes to show how important a sense of perspective is when performing any task.

I think that engineers have a major role in society, since they are the individuals who ensure everything functions as design and is safe.  The many international standards organisations show this, with the ISO and IEEE coming to mind foremost.  Without something akin to engineering, I don't think society would have progressed very far from simple tools made of wood and rock (but even that's engineering on a primitive scale!).  They have the knowledge and the skills to build any system imaginable, given the right level of instructions and leadership.

# Systems Engineering

One similarity between systems engineering and software engineering that is immediately obvious is that you need to keep in mind the "big picture" of the specifications to make sure that everything you are doing is relevant.  Both deal with large scale systems, with multiple smaller components that must interact and work together properly in order for the implementation to be correct.

Most of these little parts can be seen as "black boxes" from the perspective of other components and the big picture -- how they work internally isn't relevant to the interactions in the system.  The implementation can however relate back to the specifications in the sense of efficiency and architectures.

The two engineering perspectives also share similar process models (waterfall, spiral etc) which can be adopted as the main system process.

Thinking about the system's impact over its entire life cycle is a common trait -- in systems, this is from the start of the process to the dismantling and recycling.  In software, this begins with the basic architecture and carries through to maintainability and passing the software onto the next maintainer.

One big difference however is that systems engineering appears to be more "people-oriented", making sure everyone is on the same page and performing the correct task.  Software engineering on the other hand is more about the software system itself and focuses on the programming aspect of the system.

Software engineering also has a set of standards that are more or less commonplace across all organisations working on software systems.  Systems engineering seems to have multiple definitions that emphasise different parts of the system, and guide the overall system rather than dictate exactly how it should be laid out.  No one can seem to agree on a single standard way of practicing systems engineering.

# Human Aspects of Complex Systems

I think that the human aspect in systems can make or break its feasibility and implementation.  Nowhere have I seen this more than in my role as a Peer-Assisted Learning (PAL) mentor for computer science.  In this role, I help first year students to reflect on their learning and see the bigger picture behind the courses, as well as teach them study skills and thinking processes to use in their learning.

All too often, I've found that it's very easy to slip into a more "tutor"-esque role of presenting content and methods straight away, since students often want to shoot directly to the problem and get an answer (we're all human after all!).  I suppose that in a sense this is the "pressure" we face in the system to head towards the "unsafe" (more properly "unproductive") space of giving out answers and leading students too much -- which goes against the goals of PAL and doesn't end up providing a solution to students.

A big problem we face in PAL is that we are trying to tackle an immensely complex system -- that of trying to model and improve learning itself.  Every student is different, and the way that they go about their learning is unique across the cohort.  However, we have found that there is an underlying factor and driver to every action they take, and this is how we have been building up our model to understand where students are up to along their path of learning, and help them overcome any obstacles they are confronting.

We are constantly reviewing how we understand what is happening underneath learning and study skills, and what is really going on at a base level.  This could be related to "measuring harm" from the slides this week, since we are constantly finding new ways to evaluate what we are doing.

This leads straight into understanding the causes of the issues in the learning system -- i.e., the perceptions of the individuals concerned.  It's then our job to come up with new ways to help them with a solution, often by designing open-ended activities which allow them to come up with their own mental model rather than trying to impress one on the students, since we have found this is more effective.

I'm not so sure that the human aspects of this system can be related to the "swiss cheese" model, but there are certainly knock-on effects caused by mistakes on our part or misunderstandings on the part of the students, that can hurt the impact we have on the cohort if we don't find the cause of the problem they are facing.

In the end, I believe that everyone involved in the PAL program is keenly aware of the challenges we face, and we are creating and evolving a system to monitor and anticipate potential pitfalls in student learning, and come up with ways to continuously improve the way we run PAL sessions and help students with the unique issues they face when starting university.

# Requirements Engineering and Large Scale System Architecture

An important point raised in the panel on requirements engineering is that requirements failures are the primary cause of project failures.  I can imagine that in a large and complex system, the needs that each part of the system needs to fulfil could quickly become very convoluted and inconsistent even if they are in essence quite basic.  The amount of shareholders, and especially the communication amongst the shareholders, seems to be the biggest problem that I could face, since it would not be easy to decide on the precise needs (and the compromises that would need to be met) from everyone's point of view, rather than just a few individuals.

I think that it is easy to know when you have too few requirements to fully describe a system, since there will be holes in the system description that would become obvious either through analysis or via implementation queries later on.  Conversely however, I'm not sure that there is One True Way of knowing when you have too many.

An interesting point that was raised is that a competitive environment where everyone is disagreeing and blaming each other does not help to create solid requirements.  I've always wondered how such systems come about, since in my own experiences there has never been a time where such an environment existed around me.  I have always worked to pull other people up and support them, and have received this in return as well for the most part.  I think that this relationship of trust would be beneficial in any systems task, not just requirements, since it would focus discussion on goals and what the system needs to do, rather than protecting oneself and deflecting blame to protect integrity.

Having the right documentation to build requirements is just the first step.  After working out what the system is and needs to do, a model or architecture is essential to get an idea of cost, implementation and resource management.

Personally I've never been particularly good at this step, since I tend to rush in and attempt to solve a problem from the description rather than think about the best way to do it.  I've been aware of this for a while, and I'm constantly working on improving this so that I can design and create better systems in my programming and other areas of my career.

I found the case study from the Architecture panel to be very helpful in understanding the concept of an architecture framework.  Before this, I believed that the architecture of the system was simply a model of what it could look like at a high level, but now I understand that there is a lot more to it, with capability alternatives, and a way of showing the fit for purpose in layman's terms to help keep everyone on the same page.  Keeping it simple seems like it is again a really easy thing to get right, WHEN you know enough about the system itself, and can draw on previous knowledge to create an effective model that accurately captures the high level model.

It seems to be a mix of years of experience and asking the right questions to the right people that leads to a really solid architecture, which can then in turn become a common language between experts in different fields and other unskilled individuals.  This reassures me about my understanding of architectures, since I was quite worried that I was missing something key that other people already had.  Now that I know that it takes a lot more than just "knowing" the system requirements and people to talk to, I feel that architecture design is something that I can continue to improve and reflect on in the future without concern that I am lacking in the fundamentals.


# Model-Based Engineering

I really enjoyed this panel -- it helped solidify my understanding of the role executable models can play in software and systems design, and definitely opened the floor to thinking about future systems implementation.  The big benefit seems to be as with most systems in the automation that the model promotes.  Software is definitely eating the world, replacing a lot of jobs with automated systems.  Having a model that allows this would reduce the complexity of a project and help keep costs and resource wastage down too, since it in a sense removes the human factor from some parts of the equation where there doesn't necessarily need to be one (i.e. translating requirements that never change into code every time the model is changed).

I can definitely see the benefit of domain-specific language in a model to design the system itself, or a simulation of it.  Perhaps this is something that could be feasible with the newly popular functional languages, such as Haskell and Clojure, which lend themselves to domain-specific modelling in an easy to implement manner -- if you understand the concepts they use.  It seems that as the thinking moves up the abstraction layers, so does the skill required to implement such systems, since abstract designs require a lot of expressiveness to implement properly without getting lost in the details, and this in turn requires a certain level of knowledge on the part of the programmer to use a more expressive language.  Cue references to Paul Graham's Beating the Averages essay (http://www.paulgraham.com/avg.html) -- it's all about improving your mind and understanding of languages to develop more succinct and powerful ways to solve problems.

The ability to separate concerns at such a high level means that experts in different fields can model and interact with the system in a way that is more tangible to our abstract human thought than the way a computer understands instructions.  It means that architectures and requirements could be easily captured and changed, even if there are late additions, since the system is in a sense "simplified" to the high level abstract model, with the implementation and low-level details dealt with in a more automated manner.  I'm certainly impressed at the case study presented in the panel, and it's helped me realise that model-driven development tools is an area I'm really interested in exploring.

# System Safety

This is a topic that I think doesn't get enough attention in many software systems.  Take for example the latest OpenSSL flaw, Heartbleed, in a codebase that runs most of the Internet's secure connections!

Following standard coding principles is one way to ensure that systems and complex programs are safe enough for use in the real world.

Safety becomes especially important when there are disastrous consequences for failure -- given the diversity of opinions on a topic however, and the likelihood of failure happening, sometimes these are not taken into consideration.

One of the big sources of failure in systems (and getting messages across in general) that I have seen so far is experts in one area attempting to implement a system in another area that they are not as familiar with.  Take for example, experts in cryptography and mathematics attempting to build a secure computer protocol (OpenSSL).  The concept of cryptography is simple to them, and the requirements of the system as a whole are quite clear.  However, the OpenSSL implementation of the system has bugs due to bad coding practices, and a convoluted logic path that was implemented without any safety checking on the part of people who were not experts in programming, but in mathematics and analysis.  This links back to human factors in systems and why they can fail, since the OpenSSL committee had an idea of the platform they wanted to create, and had created a suitable design, however did not implement it safely -- leading to a model that is filled with (quite serious) holes that compromise the integrity of the system with potentially disastrous consequences.

I'm not saying that I can do much better at the moment though -- I'm still learning about defensive programming styles with concurrent and network-based programming, where one must check every return value for sanity and safety purposes.  I am trying to develop "safety nets" when I design and program systems, to ensure that the safety cases the system should meet are implemented -- something which goal structures seem to help encompass.  I'm not sure how useful this approach is in small projects, however when there are critical entities at stake I think that they are a good start towards building a sane and safe system.

I do wonder how much importance we will place in formal proof methods in future systems design.  There are already programming language implementations such as SPARK-ADA that attempt to automate the safety and sanity checking process to help write defect-free code, and given the possible future of model-based engineering practices, this could be further integrated again into systems implementation.  I think that as formal proof methods become easier to implement, the safety cases of a system will be taken into account more seriously, since there will be enough time and feasibility to implement them -- something that is sometimes difficult with current software systems, even if the arguments put forward are compelling.

Sustainability and System Dynamics

These two aspects of systems engineering are very high level, and take into consideration everything above to highlight the big issues systems need to take into consideration.  The big problem that the world is facing at the moment is the overuse of resources that are not replaceable.  The sustainability of the systems we design is therefore more important than ever, since there are planetary boundaries we just don't want to cross if we want a world for the future generation.

From a computing perspective, the way software is automating everything has been a massive boon for productivity and the development of the human race, but it has posed the issue of pretty much strip-mining everything for profit, without a care towards what happens in the future.  The way we can make this more sustainable is looking at the way technology is revolutionising whole industries, with new flexible systems reducing lock-in and having more pervasive effects on our cultures.

There is also the issue of what happens to those who are left behind by technology, since as the latter becomes more and more powerful, it is automating jobs that are higher and higher up the skills chain.  This is going to be a very hard problem to tackle, especially since the "system" at stake is the human workforce.  There are bound to be plenty of attempts to fix it that fail horribly due to social or equity issues, and I'm not really sure how we are going to tackle this problem in a sustainable manner.

In any case, reducing consumption and our dependency on massive amounts of energy is going to be essential moving forward.  Showing this to the average person however is difficult, since as was mentioned in the panel on system dynamics, most people don't understand how flows (or the rate of change) work.

I found that stocks and flows were a great way to visualise the information about inputs and outputs of a system.  I hadn't really thought about their use outside finance before, but they're definitely a really easy way to show anyone unfamiliar with a system what's happening and what needs to occur. One thing that all of us (aspiring) systems engineers need to all do as a collective is to educate people on what the difference is between stocks and flows, and the need to reduce input to a stock to nothing (instead of stagnating it) in order to prevent further growth and consequences.

# Conclusion - The Big Picture

I've certainly learnt a lot from taking this course, and it's helped consolidate my knowledge in some areas, while opening new questions and pathways in others.  I think that there is a lot of reflection required when thinking about systems engineering, and in that sense it is similar to what I do in PAL to observe and help improve my (and students') knowledge there.

I can link also link the new information I have gained here to my student ambassador role at ANU, especially since I have been trying to include it when teaching high school students about the problems they can encounter in systems engineering no matter what the discipline, and help them discover ways to think about modelling interactions internally and externally to more easily see what is happening.  I'm also trying to help people understand that software engineering and computer science as a whole isn't just about the code -- it is so important to think through and understand everything you are doing, and make sure that it matches what you need and/or want.

In the end, I think that the biggest points of failure in a system will always be people-related, whether they're due to vested interests, or differing goals, or just misunderstandings.  Whilst this is most prevalent in systems engineering in general, from a software perspective it happens all the time when working on a shared codebase.

When I first started this course, my view of software engineering was that it was all about designing a program from requirements and a general idea of the architecture it was running on.  I now understand more about how it fits into the big picture, especially communications-wise with other experts in differing fields, making sure that everyone is on the same page.

If I was to take away one thing from this course, it would be to drive home the necessity in software engineering of getting the early, high-level requirements and model right before continuing onto implementation, so as to ensure a sustainable and productive system that is safe, sane and understandable to everyone.