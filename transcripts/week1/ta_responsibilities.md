So what are the TA's responsibilities?

We've developed a TA's Creed, which you should know if you're going to be a TA.

Four combined things that you need to be as a TA.

You need to be responsible. 

If there's a problem you need to pass it up through the chain of command.

Respectful to the students who are struggling away with the sometimes difficult and challenging material.

You want to be "on topic", relevant, informative and resourceful.

Students will get stuck in this real-world software; they'll get stuck all down different sorts of alleyways to do with the version issues and libraries and so on.

You'll want to think on your feet, get the right sorts of information to the right people at the right time.

One of the key things really is to be actively engaged with the courseware.

Particularly if you took the 169 course some time ago then you may not have the assignments and the aspects of it in the forefront of your mind

Ideally you need to be working through the courseware with the students so that you've looked at the assignment and just completed it, i.e. the one they've been working on that week.

You also need to be a facilitator.

Rather than just solving problems; you need to help other people solve their own problems and we'll talk more about that as we go on in this next section.

[NEXT SLIDE]

In terms of supporting students what we really want is the students to becoming more and more independent of the TA's and the instructors and so on.

We want them to become independent learners.

So we want as much as possible to help them discover the answers by themselves.

Rather than just saying: "this is how you do it, and then you do this, and then you do this", we need to provide a scaffolding.

A scaffolding that is about helping them learn to discover the answers by themselves.

We'll get into that in more detail in a minute.

Another key thing is helping them get past needless roadblocks to learning.

There are certain points where, and this is sort of a judgement call between whether they are stuck because this is a version issue;

And we just need to fix that so that we can focus on a higher level software engineering issue ...

Or is it actually that this versioning or library issue that through a process of exploration they could solve by themselves.

And knowing which is an intuitive thing that you will need to develop over time.

It's good to be aware that there are two sides to every problem.  Some maybe just to be fixed if the learner is too stressed, and the problem is not related to the current learning objective.

But in other cases almost any problem can be used as a springboard for learning, and helping a student become an independent learner. 

Naturally providing correct, relevant, and clear information is absolutely essential

Furthermore we also want to maintain a culture of collaboration, because a positive process of collaboration is fun and helps people learn.

So it's essential that we help students help each and support each other.

We definitely want to get as much of that as we possibly can.

[NEXT SLIDE]

So there's a number of different forums where students will be communicating with each other.

We've got an asynchronous bulletin board in the form the edX forum.

We've also got live realtime chat, that is embedded into the HTML of the site - that's using Gitter: a GitHub based chat client. 

The key thing in any of these forums is to maintain civility, we're all professionals, we're all adults.

There's no reason not be polite to each other we're all trying to work together to try and improve our knowledge and understanding of all the materials.

So let's be civil. 

We also suggest cutting off unproductive discussions.

That's again a judgement call about what is a productive or an unproductive discussion.

I think a light touch is generally the way to go but if things really are descending into less than civil tones or getting widely off topic them that's a good time to try to wrap that discussion up.

Also, being helpful without just giving the complete solution.

I mean someone could say "I'm stuck on homework two" and you say could right "Ah here is the entire solution for homework two" which is arguably "helpful" from one point of view but it's not necessarily helping the student master the material.

So try and and be helpful without giving away the solution.

Keep the different threads and the discussions on-topic.

We've touched on that already.

Really try and make all the forums and the chat hangouts a place that students can enjoy going to for discussing the class topics.

We all want to have fun, so that's key :-)

[NEXT SLIDE]

Now let's talk about this scaffolding concept which you may or may not be familiar with.

There's this idea of instructional scaffolding which as I've alluded to already, is rather than giving somebody the solution straight away, it's about giving them more "temporary" support.

Just sort of helping them a little bit.

A sort of trivial example might be that say you were learning a new language and you're trying to remember the translation of a word and somebody gives you the first letter of the word, instead of the whole word.

There's evidence to show that this partial scaffolding will help you recall the same word yourself more easily next time around.

So that intervention is a "scaffold".

You're not telling the learner the complete answer or walking them step-by-step through the task.

You're helping them figure out how do the task on their own.

It's about rather than just "give an answer" to what the students ask for; it's about helping them think for themselves by asking questions.

The idea with it being scaffolding is also that it can be gradually removed over time. 

So as time goes by so you can gradually give less support.

You personally don't necessarily have to be involved in removing that support.

Your ongoing involvement with an individual learner will depend on the extent to which you re-interact with different students as the course goes on and in a course as large as this maybe you won't interact with the same student again.

However, the idea of the scaffolding is at least it's there for support at the beginning and then ultimately the students by the time they graduate the course they don't need that scaffolding anymore and they can get by on themselves.

[GET READY TO PULL IN RUBY CONSOLE]

I want to give a quick example with Ruby.

[PULL IN CONSOLE]

Over here I've got the command line and this is sort of a trivial example here but let's say that we've defined some method in Ruby like so

[TYPE OUT RUBY METHOD DEF IN IRB]

And a student has unwittingly made a call to that method like this 

[TYPE OUT RUBY METHOD CALL IN IRB]

and they're saying "hey look, I'm getting an error, I don't know what's going on"

Now if you know Ruby reasonably well this will seem pretty simple and you might be tempted to say: "oh yes I know exactly what the problem is"

And you might be tempted just tell the student the fix.  You could just say "oh right you need to redefine the method with some arguments" and you could just give them the solution.

A more scaffold based approach would be to start asking some questions like: "okay so ... what are you actually trying to achieve here, what's the high-level goal?" which might seem odd here, but becomes more important as things get complex.

And then you say "so does any part of the error message make sense to you?"

And depending on what they say you direct them to the part of the error message that says "ArgumentError: wrong number of arguments" and ask "does that mean anything to you?"

So rather than saying explicitly "you need to add arguments to your method definition", you can be asking if the students knows what argument is? 

Or better yet, waiting for them to ask you what an argument is.

Maybe the student has already carefully read the error message and they've just no idea what arguments are.

So then you can say "well arguments are things that you pass to a method" and maybe show some examples and then say "there's the wrong number of them in this case".

As before this is a judgment call about at what point to intervene with what question or information.

How much scaffolding should we give?

I mean it can be frustrating for the student if it seems like you're asking too many questions.

Its something that you have to to build up an intuition for over time.

Note that this is also the same sort of support that a senior developer might give to a junior developer in order to help them grow as a developer.

Although in a project with a paying client you've got to balance what's best for learning against what's best for delivering the product in time. 

Anyhow, you can also read lots of materials online.

We'll post some links for other reading on this topic on instructional scaffolding.

In summary, rather than just providing answers you want to help pose questions to the learner that allows them to discover the solution in their own way.

So that next time they have a better chance of solving a similar, or even a more difficult, problem without any support.


[NEXT SLIDE]

Also you need to know how to connect with the team and there's certain critical things to do.

Checking into and out of the AV102 Slack chat.

We have a chat room in Slack so as you come online and you should post and let us know "I'm going to be checking the forums" or "I'm going to be hanging out in the Gitter chat"

So you check in and when you've finished answering student questions or what have you, then you check out in the Slack chat; saying "I'm finishing up for now"

This is really all about announcing that you're on-duty because there's an extent to which if we have 200 TAs and all them are on duty at the same two hour period then that's not very effective way of serving the many thousands of students.

So we want to have a mechanism whereby we let each other know when we're working so that as we're checking in, if it seems like some other people are already active in the forms and chat then, you can say to yourself "Oh I'll come back in a couple hours instead and try and contribute then"

So you need to monitor these various when you're on duty communicating with the various members of the teams as you do.

So you want to mention in the AV102 Slack chat when you're addressing a students question, by posting a link to that question. 

That will help avoid many TAs trying to answer the same question at the same time independently; and draw them together in slack to collaborate on an answer if necessary.

[NEXT SLIDE]

Another thing that we're keen for you to do is to encourage the students to pair program with each other. 

As in previous versions of the course we have a framework for students to do pair programming together. 

One of the key bits of feedback that we've got from that is that it's often difficult for students to get themselves started sometimes.

So we're really keen to have TA's help students get started with pair programming:

Starting a session, for example, if you've got too many students in the same session encouraging them to split off into pairs who are working on the same parts of the same homeworks and so on.

Explaining the idea that they they shouldn't be just posting complete solutions, or taking copies of solutions if they've just joined the end of a pairing session.

One of the best ways you can help here is ensuring that you've done as much pair programming yourself as possible, and sharing tips on what you find helps it work well for you.

[NEXT SLIDE]

Of course one of the most critical things is to be engaged.

I think if you really want help students you probably want to actually re-do the assignments the week before the students do them; in pairs if at all possible :-)

I will give everyone, i.e. all the TA's, beta access to the course.

That will mean you'll be able to see the course materials a week in advance.

I think one of the best ways to give the most effective help to the students is if you do the homeworks early in the week and then that's in the forefront of your your mind.

Also if you're doing the homeworks in advance you can also submit them to help us check with the auto graders.

Please report any bugs through pivotal tracker.

We'll give you access to pivotal tracker to report those.

Also if we've got critical errors such as the student Gitter chat not working or the auto graders not working or anything then please escalate it by posting links to the tracker ticket into the AV102 slack chat by typing @tansaku.

Which will alert me, Sam Joseph, which is where the buck stops here with making all these things work :-)

Note that this is also an important part of working in a distributed team which is reporting errors through an issues tracking system like pivotal tracker and then including the URL to that issue in digital communication like chat and email etc.  

This is essential to ensure that everybody working on a given problem has access to all the relevant information.


TODO

* resource links for helping junior devs, instructional scaffolding