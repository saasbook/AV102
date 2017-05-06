Welcome to this week on "Distributed Software Development".

Distributed Software Development means the process of software development, which we all know and love; but involving individuals who are distributed in diffirent physical locations, potentially all around the world.

This week we're going to review several software tools that I think many of you will already  be familiar with from the 169 course.

Thus this week is a bit of a refresher in some ways. Next week we'll connect up more  strongly to team practices.

Although I will do my best as we go through to mention the connections each tool or concept  has to distributed team management.

Anyhow, many of these things we're going to talk about this week are just as valuable  for the opposite of "Distributed Software Development",  that is: "Centralised Software Development".

By Centralized Software Development we mean what goes on in your startup or your company  where you have a room, or a floor, full of people. 

All the team are there together and they can quickly jump into a meeting room and discuss  what they're doing.

Also, they can bump into each other over the water cooler and so on.

So anyhow the software development techniques we're looking at this week are incredibly  valuable in whatever way your team is set up.

Several of them are key concepts from the Engineering Software as a Service course that  I want to pull out, partly because it's good to have a refresher on them;  partly becauase they are the kind of things that many MOOC students get stuck on, but also because they are critical compoents of working effectively in distributed teams.

So I believe that having all of these concepts clear in your mind will be extremely helpful.

And while some of them valuable are very valuable in centralised software development settings,  I think they're *particularly* valuable in distributed settings.

So let's just give you a quick overview of what's coming up, we've got these videos,  and first of all we're gonna talk about user stories:

That's the process of ensuring that the work you do actually meet customer needs, rather  than just being what you think is cool.

This might seem like a sort of wishy washy thing, but I think the really clever person,  the really really clever person, works out not how they can use a set of technical tools  in order to solve a problem; they work out what the problem really is.

In particular they work out what's the minimum intervention that would satisfy the customer.  

Sometimes the best solution is one where we say "actually we've worked out there isn't  a problem here and thank you very much",  and you get paid a large consulting fee for having worked out a way of solving things  with slight modifications to existing systems and processes.

However, more often than not, people will want custom solutions to things and so you then you'll be  collaborating with others while using your toolkit of different coding skills and knowledge of different frameworks.

Still the key thing is that you have to get the user stories sorted up front; sorting  out the wheat from the chaff so to speak.

You've got to work out what the customer really needs, even when they aren't sure themselves  and that's what the process of developing user stories is about.

Then there's user stories versus chores. 

Chores are bits of infrastructure work that have got to be done; and you need to track  and coordinate them.

So that's the start of this week: user stories and chores. 

What we're trying to do here is represent a bit of the flow that you might follow working  through a real project, which is for example, on inception, you will be starting with user  stories.

Then having developed those user stories with the customers and other stakeholders you'd  be also realizing "aha these various chores have got to be done too". 

And then you'll say right okay well we'll put off some of these chores. 

Here let's just start working on the first two user stories we think that are key for  our MVP or Minimum Viable Product.

And then you can start work and you might actually start coding with, let's say, Cucumber  or RSpec doing your acceptance test and then even getting down to the unit test level.

This acceptance/unit test cycle is also very important; this process of getting red  acceptance tests, red unit tests and then going green is absolutely key and we'll go  through that in more detail this week. 

It's absolutely essential for quality control.

There's also the process of communicating with the team through the codebase itself.  

I believe, along with Armando and many others, that the documentation is not necessarily  worth the paper it's written on.  

What we want is *live* documentation, which is your acceptance tests and your unit tests  that explain what's happening in the system.

That's just absolutely essential and creates documentation that can be verified by running  it against the code.

So that's important for quality control and communication with the rest the team.

Again, whether you're distributed or centralized it doesn't make too much difference,  but again I hope you can sense the arrangement of this week's materials reflects the flow  you might have in a serious project.

Version control then comes in, given that you want to be able to undo people's mistakes (especially your own).

Then you further develop the user stories, the acceptance and unit tests etc.

Even the user stories themselves should be going in version control.

Anyhow, a really good understanding of version control how to use distributed version  control systems like GitHub; that's systems that allow every team member to have access to the codebase, is absolutely essential these days.

Futhermore, many of us will also be deploying to the cloud, through git or other version  control systems.

So once you've got "version one" of your system you'll want to get that up in the cloud. 

Thus we'll review the Heroku "Platform-as-a-Service" and then finally this other concept  which we think is critically important, which is this idea of "spiking".

"Spiking" refers to quickly developing a prototype that you're then going to throw away afterwards.

I think back in the day as, I say in the actual video itself, that was what everybody did  all the time.

There were almost no tests and all code was one big spike.

You might say shouldn't we avoid that at all costs, but I think it's good to have a name  for it.

Then when you're talking to members of your team; or as we're talking with with students in  169 we can talk about "oh right what you were doing there was a bit of a spike".

"Now let's stop that and go back and do a really rigorous acceptance-test/unit-test cycle as we move forward".

So that's the overview for this week.

I hope you find all this of some interest and that they're nice refreshers. 

Apoligies in advance that I haven't been able to re-record all of this week's videos.

I have managed to add full transcripts for all of them, which I hope will help make them  more comprehensible.

As you'll be able to tell, the upcoming videos were recorded somewhat off the cuff and a  year or two ago.

There are other things I'd like to update, such as to the latest RSpec 3 syntax in the acceptance-test/unit-test video,  but I think the concepts are still sufficiently clear and so at the moment I am prioritising completing subtitles for all the videos in the upcoming weeks.

Also in some of these videos, I do go into some live code examples, so those videos do  run a bit longer.

I think those are valuable in that you can see me making mistakes and recovering from  them, which is kind of the core skill.

It's really important for learning that we understand making mistakes is natural and  human and we all do it, and it is how we learn.

Anyhow, please do feel free to watch as much as or as little as you prefer.

If you took the course recently and you're working with all these tools and techniques  regularly you may say "right, I kind of know this stuff already".

Feel free to watch as much as or as little as you need. If you took the course recently and you're working with all these things regularly you may say right, I kind of know this stuff.

Obviously it's entirely up to you whether you watch the videos and do the little quizzes  at the end,  but what is required if you want to get the certificate is this week's assignment on Github  and Heroku and working with git;  just to make sure you're on the tip top of the skills.

These are things which I think are very very important; both for working with distributed  teams and of course for the ESaaS MOOC.

Okay, so, I hope you enjoy this week and I look forward to continue making your acquaintance  in the slack chat; it really is great to be meeting so many of you there.

Alright bye for now.
