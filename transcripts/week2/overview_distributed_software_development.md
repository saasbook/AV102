Welcome to this week on distributed software development, which is a title which we've struggled over and it's a relatively new term. We're using it to talk about the process of software development, which we're all interested in, but involving individuals who are distributed around the world.

This week we're going to review many of the software tools that I think many of you will already be familiar with from the 169 course.

That makes this a bit of a refresher in some ways, while next week will connect this up more strongly to team practices.

Although I will do my best as we go through to mention the connections with distributed team management.

However, many of these things we're going to talk about this week are just as valuable for what we might call the opposite of distributed software development, i.e. Centralised software development, for example git and GitHub and Heroku and the acceptance/unit test cycle and associated techniques.

By centralized software development we mean what goes on in your startup or your company where you have a room or a floor full of people and they're all there together and they can quickly jump into a meeting room and discuss what they're doing and they can bump into each other over the water cooler and so on.


So these techniques are just fundamentally really valuable and several of them key concepts from the Engineering Software as a Service course that I want to pullout, partly because that's a good refresher, partly because they are critical compoents of working effectively in distributed teams, but also because I think these are the kind of things that many MOOC students get stuck on, for example aspecs of git and GitHub and Heroku and things like that.

So the clearer those ideas are in your head then (and with a nod to each of our multiple course goals): 

One; it'll help you manage distributed teams better
Two; it'll help prepare you for being a teaching assistant in the 169 course  AND
Three; it'll help you take part in a distributed team.

So I believe that having all of these concepts clear in your mind will be extremely helpful

And while some of them valuable are very valuable in centralised software development settings, I think they're *particularly* valuable in distributed settings.

So let's just give you a quick overview of what's coming up, we've got these videos, so first of all we're gonna talk about user stories:

That's the process of focusing on getting the work done so that you can really meet customer needs.

This might seem like a sort of wishy washing thing but I think the really clever person, the really really clever person works out not how can I use a set of technical tools in order to solve a problem; they work out what the problem really is.

In particular they work out what's the minimum intervention we can make to improve things.  

Sometimes the best solution is one where we say "actually we've worked out there isn't a problem here and thank you very much" and you get paid a large consulting fee for having worked out a way of solving things with existing systems.

However, more often than not, people will want custom solutions to things and so you have to start bringing in your toolkit of different coding skills and frameworks.

Still the key thing is that you have to get the user stories sorted up front; sort out the wheat from the chaff so to speak.  You've got to work out what the customer really needs, even when they aren't sure themself and that's what the process of developing user stories is about.

Then there's user stories versus chores. 

Chores are bits of infrastructure work that have got to be done; and you need to track and coordinate them.

So that's the start of this week: user stories and chores. 

What I'm trying to do here is represent a bit of the flow that you might have working through a real project which is that on inception you will be starting with user stories.

Then having developed those user stories with the customers and other stakeholders you'd be also realizing "aha these various chores have got to be done too". 

And then you'll say right okay well we'll put off some of these chores. 

Here let's just start working on the first two user stories we think that are key for our MVP or Minimum Viable Product.

And then you can start work and you might actually start coding with, let's say, Cucumber or RSpec doing your acceptance test and then even getting down to the unit test level.

This acceptance/unit test cycle is also very important; this process of getting red acceptance tests, red unit tests and then going green is absolutely key and we'll go through that in more detail this week. 

It's absolutely essential for quality control.


There's also the process of communicating with the team through the codebase itself.  I believe along with Armando and many others that, the documentation is not necessarily worth the paper it's written on.  

What we want is *live* documentation, which is your acceptance tests and your unit tests that explain what's happening in the system.

That's just absolutely essentially and creates documentation that can be verified by running it against the code.

So that's important for quality control and communication with the rest the team.

Again whether you're distributed or centralized it doesn't make too much different but again you can see this sort of flow here where we go from how you might actually go through the project.

Version control then comes in given that you want to be able to undo people's mistakes.

Then you further develop the user stories, the acceptance and unit tests etc.

Even the user stories themselves should be going in version control.

Anyhow, a really good understanding of version control how to use distributed version control systems like  GitHub that allows everyone to have access to the codebase is absolutely absolutely essential these days.

Many of us will also be deploying to the cloud through git or other version control systems.

So once you've got "version one" of your system you'll want to get that up in the cloud. 

We'll review the Heroku Platform as a service there and then finally this other concept which we think is critically important is this idea of "spiking"

"Spiking" refers to quickly developing a prototype that you're then going to throw away afterwards.

I think back in the day as I say in the actual video itself that was what everybody did. 

All coding was entirely spiking but I think it's good to have a name for it.

Then as you're talking to members of our team; or as we're talking with with students in 169 we can talk about "oh right what you were doing there was a bit of a spike". 

"Now let's stop that and go back and do a really rigorous acceptance test unit test cycle as we move forward"

So that's kind of the overview.


I hope you find all this of some interest and that they're nice refreshers. 

I know that I do speak too fast so you can speed me up slow me down with the player controls which are down there somewhere.

In some of these videos, I guess it was this one with the acceptance tests, version control, deployed the cloud, I do go into some code examples so these have got a bit longer.

Feel free to watch as much as or as little as you need. If you took the course recently and you're working with all these things regularly you may say right, I kind of know this stuff.

Obviously it's entirely up to you whether you watch the videos and do the little quizzes at the end but what is required if you want to get the certificate is this week's assignment on Github and Heroku and 
working with git; just to make sure you're on the tip top of the skills.

These are things which I think are very very important; both for working with distributed teams and of course for the ESaaS MOOC.

Alright well, I hope you enjoy this week and I look forward to continue making your acquaintance in the slack chat; it's great to meet so many of you. 

Alright bye for now 