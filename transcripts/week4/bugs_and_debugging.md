https://edge.edx.org/assets/courseware/v1/e7b54efbd97baf28995197e4ab96b2d7/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/4.2-_Bugs.pdf

Hey so let's talk about bugs and debugging ... bugs
happen. They do; and sometimes they're very worrying ...
why do bugs happen? I guess there's this phrase
human error ... we humans
we don't always respect exactly the logic or the syntax
of the computer system we're working with ...
although I would say in some ways
... if ... in the ideal world
we as humans could just carry on behaving in the way that we like behaving
maybe irrationally, illogically, what have you and
the systems we are working with would just ... would
interpret that ... unfortunately
our computers are still distinguishable from magic and they can't
quite interpret what we want and so they have these ... rules, logic
syntax that we
kind of ... if we want to get them to do something we have to kind of - 
if we want get them to do the thing that we want them to do
we have to sort of end up respecting those so ... we're gonna make
slips
where we fail annoyingly to match the logic or the syntax
... of those systems ...
other things might be going on the background. There might be a change in
environment
yeah ... your operating system is upgraded
... configuration is changed. I mean this is why
we release the virtual machine it's to try and have a single
stable environment for everybody to work on, single configuration
but we use a tool like bundle to manage all the gems
for the
different software libraries that are needed to do all the different bits and pieces
and this ... in some ways ...
... the programming and even the testing bit
and even the BDD and so on; it's all relatively straightforward
sometimes compared to trying to manage issues that kind of come up in the environment or the
configuration
and so on ... and sometimes it's just a difference in -
in perspective ... you just ...
there's bugs at the software level, there's bugs at the interface level;
is it just that you thought something was going to work this way and
it actually it should work that way ... I mean just
stuff happens ... I've got a few slides here that are mainly focused on
kind of bugs from the software perspective and I mean this is - this is generally also it's ...
we're following
from the textbook ... there's a great section
... which I've just got over here ...
which I think is, is it 4.7? Oh, where's that table of contents - it's
four-point five: debugging when things go wrong
I think almost could be broken out into its own chapter ... in some ways
this is the key thing about ... dealing with technology being a
software engineer
is about your process that you use
when you encounter an issue; whether it's an interface issue or a software
bug ... there's a - something is broken (or test is failing).
And the key thing is
as Douglas Adams would say is just "Don't panic!" Really, ...
and of course it's difficult when there's a deadline and there's eight other team-members saying "We must have this now!" "We must
have it now
now now!" ... it's challenging ... we have
... we all have at any given time a model in our mind of how
the technology we're using is working and have expectations and when
things are different from those expectations it's like Errrrrrr
and the key thing, assuming that you're getting some sort of error message,
is to read that error message ... sometimes that error message might not
have the information in it that you need sometimes ... there's no
guarantee but do
read it ... I mean it's the kind of thing ... you can get thrown off track of course
... the error messages are also something that are designed
to a degree by the developers of the system
developers of the systems whether it's a website, a web app,
a programming language a compiler whatever it happens to be; they're
doing their best. There's often
we get frustrated with ... computer systems
whether ... technologies - because they don't ... it's like
"Ooh the person who designed this! They're not seeing
things from my perspective!" No, I mean ... they were doing their best
... I think
... other things being equal shall we assume that they were doing
their best? They maybe ... not being omniscient, as developers are not,
didn't necessarily see precisely the way that you were
expecting to use the technology, or maybe they did, and just other things have changed and they
haven't worked out how to get the error messages
to ... be as comprehensible as they could be
although I say I think there's a tendency, at least I have from - from using Ruby and Cucumber,
I think the error messages are getting more helpful over time
rather than just being a strange Pig Latin thing; or maybe that's just a question of me getting more and more familiar
with them
but I think there's more ... there's a tendency now to put English language instructions
in the error messages and have suggestions of what to do ...
but one of the things with a software bug is you might well get a backtrace and
I'm sure you're all familiar with that ... which
tells us where things went wrong and what went wrong
... this is one of the things ... this is a
refresher for all of you. I'm sure you guys are all dealing with backtraces
every day.
Certainly for the students coming into the MOOC
and indeed maybe new developers on your distributed team
may not have ... I guess
one: the necessary experience with backtraces to kind of use them to figure out
where things went wrong or what went wrong
... and they may often be sort of telling you " Oh, I just had this problem" and
they won't show you the backtrace and well anyway
more of that soon. Sometimes there's no backtrace
and that's when it's in a really good ideas to check the log files
... a common issue from the MOOC was
people get an error in Heroku and you need to type 'heroku logs' to see the
logs files ... and I ...
actually that's an interesting one with Heroku in that
I would argue that maybe when you deploy your
Heroku app by default it should have -
you know - a setup so that the backtrace is
displayed by default ... there's -
we can always sort of push this thing around.
One thing overall as you know we're working with the tools that we have
and ... we do the best we can. Actually from
Heroku there I've got an example backtrace
that you may have ... easily have students
encountering in the course ... you may have encountered yourself when
trying to deploy to Heroku;
and the problem with these stack traces and I've actually taken ... this is just a
portion
of the overall stack trace the came up during a Heroku deploy;
and the challenge ... which you've probably discovered yourself is that
there may be ... in there ... you've got like
deprecated ... there's warnings that may be not critical and not related to the
failure that you had
... there's ... other bits of the stack trace
which have a lot of the same information repeated because there was a nested
calling operation and so on ...
probably ... since you've reached this
point in the course you've ... and you've passed the previous courses
you've encountered these sort of things before; but so it's
.. but for a novice and for a junior developer
this can be like a horrible sticking point and you might say well
just search for it ...
on Google and the temptation might be to take the entire thing and just say "I just don't know what's going
on and there's this thing and it's like no no right, I .. it doesn't help and
look there's been an error on Google and just oh ..." I mean
this is the point at which we all need support; you've got -
you've got error
compounded upon error. The approach as
I'm sure that all of you know is to kind of calmly work through this
and read "okay deprecation warning, you have a Rails 2.3 style plugins in vendor ...
support will be removed ... I mean part of thing is knowing that warnings
are there and won't be the source ... your main source of the problem.
A message look there's rake aborted could not connect to server, connection refused
is the server running on host ... and accepting
TCP/IP connections ... for me the
instinct; okay that looks like the load-bearing
part of the error ... in this case the stack trace
NOT so helpful for telling me where things are going wrong, I know it's sort of -
its related to the database here. If I then go and search for that
in Google aha! Aha! There are Stack Overflow I always love StackOverflow
... posts because ...
our great friends at StackExchange make sure that people are able to
vote the correctly
... correct answer or the most useful recent answer up
to the top and we find that there is actually a fairly simple fix
for this. Although you can back up and say
well hey! And as I think as we
will be trying to do in this next run of the course is make sure that
... things like this are pointed out. I mean this actual error that I
got there is from a walkthrough
on chapter four from the text book ... let's just go
into the ... virtual machine here
... and yeah it was part of a much
longer error and it's one of the things that if you, for example, if you do the walkthrough in chapter four
and then you try and
deploy MyRottenPotatoes to Heroku, unless you've set this particular variable
then and I think we might have encountered the same issue in one of the earlier
lectures ... let's get rid of that for the moment. Yes
yes - so I mean there's ... we're also
delivering this course doing our best to try and make sure that these
issues are not encountered and that the ... to a certain extent the students can be
focusing on
the I guess you might say that the key software engineering
issues such as the red green and refactor and the behaviour driven development and so on.
We don't want people to be stuck
staring at this and saying I have to submit this homework or I have to get this
site out for my client and I just don't know how it works and the I'm
stuck
... to the extent possible we don't want people encountering these things
but as ... we're using a real professional developer's stack here as time
moves on
... this one maybe we'll have fixed and all sorted for this next run of the
course.
I'm sure new things will come up. So part of what we're doing with
the learners with the junior developers on our teams is scaffolding them through the
process
of staying calm and learning the intuition of when things go wrong
what are the important parts of the information the computer is giving us
that we need to focus on ... if we go on
I mean this is diagnosing errors
... particularly with a focus on Rails
views here ... which is -
is fairly common in this course - we can put
instrumentation in the view so if we've got a running ... and I have
got a running ... so like for example
variable.inspect() or what have you we can ...
I've got set up to show the next slide but ... I've got a ...
if I just shut that down there; I've got
this is the MyRottenPotatoes as you would get to it at the end of
...
I've got confused about ... there's the editor; as you would get to at the end of the
chapter 4 in here ... and we'll look at debugging the controller
again momentarily, but so if we look in a view ...
let's go into a view and there's the index there so
I'm not such a big fan of HAML but we can do things
here ... actually is that set up for HAML ...
hmmmm ... like variable.inspect() or debug variable
I'm probably going to end up ... well we might get an interesting error whatever I do here
... I wonder if it will let me ... see if I want to
get the code do I need to ... I need to do
just like the percentage ... see I'm really not such a big fan of
HAML. There can I do debug
@movies like so?
Ooh HAML ... and then see if I go and run,
go and run the server there. 'rails s'
And then let's reload this and we'll ... at least we'll get ... even if it doesn't do what I expect
we get a ... this is I mean in some ways this is ...
at least here with this layout is giving us
more. It's not just throwing ... like Heroku might do at the beginning.
It's not just saying oh something went wrong, we don't know what it is and you have no idea
where the log file is
for that or what have you; but so we can see here
that yes, my debug operation there is not working
... we could just go and quickly ask the question
debug in HAML views
... [HUMMING] ...
yep ...
ah yes, HAML HAML HAML yes, I think what we need is we need critically
actually a tag that goes with it; so I think if we
save that and rerun that
... yep, there we go
so ... we're getting our page there we've also got
we're dumping ... the debug output of our movies
movies there ... not a big fan of HAML myself
but there we go; so that's yeah -
we can be writing to the log file, we can raise an exception
... my personal favourite really really would be ...
these kinds of things are okay I would much rather use the debugger
to stop and examine the state of what's going on.
The debugger gem ... it's funny I personally never seem to need to use
this running the rails server with the debugger like so
but this is the kind of thing that I went through in
my various ... I guess Helpouts
or course ... I've forgotten what I call them but every week during the last course you may remember I
was sort of
making myself available in Hangouts to go through peoples' problems.
I think often the debugger, particularly when you're getting stuck on this debug
loop of changing some code and reloading everything
just like being able to ... and I'll just, at
the risk of repeating myself, if we go in here and we say that we look at
at - as it was earlier, if we go in here in the movies controller and we
place a debug statement in there I think I've already got
a debugger in the gem file ... yep
in development and test ... and so if we've got
the debugger in there ...
I think I've got ... I'll just shut this down ... I find
the minus minus debugger seems to not be necessary. If I now run
here ... I think we'll see that it gets stuck on the debugger there
quite easily and I've now got this environment here
... I'm in a sort of debugger; I can jump backwards and forwards in methods and so on
... in particular I can go into this sort of 'irb' thing and I can expect
... sorry inspect, interactively
what movies is at that point. Oh it hasn't actually been run because the debugger stopped there so I could
even
copy and paste a little bit of code ...
fill in the variable there and I can do the movies
size and so on and having that full
interactivity there in the immediate loop, so absolutely hugely hugely
valuable, can save so much time
... so one of the things ...
generally I find often ... whether it's on a distributed team
and they've got stuck on a cycle and I say "Oh let's jump in
with the debugger"
... whether it's a student online it's like
let's get in a Hangout and screen share and let's hang it on the debugger
and actually see what's going on ... you can solve things
very fast I think compared to these alternatives where you're
doing a lot ... inspecting things and so on but you know
... the debugger has got more moving parts; there's other
little things that you can run into for example that if you put ...
the debug statement ... here
instead of here, then it doesn't necessarily ...
that's ... kind of goes a bit crazy usually
... always try and avoid debugger being at the very end of the line
that you want to have it ... at least one before
the end of the line, in my experience with debugging Rails and Ruby
... so moving on ... so there's the tools
... avoiding the bugs ... I can't ...
this is just huge like having ... automatic indentation
and highlighting to avoid syntax mistakes; that's ...
I think ... I guess I use ... I lean on
automatic annotation less than I to used to
I tend to be ... the VM that
we distribute comes with this GEdit ... it's got
you know you get the tab width and so on set up. I don't think it has a function for
auto-indenting all these things. If I'm
in my preferred - 
RubyMine - Do I have a RubyMine at hand? So yeah -
I can be in some code and I think it's ... what
is this command is it like that to ... it
used to be that Eclipse was the thing that I loved for automatically indenting
the code
I think I now, oh yeah, there's reformat
auto-indent lines, yes that's the
is it actually the control alt L?
control alt auto-ident yeah... I end up not
oh goodness me I've accidentally
I think I've accidentally turned on inklet there by mistake ... I tend to rely on that less
... the key thing for me whether it's automatic indenting or not
is I just, I'm always making sure that my indenting is -
makes sense ... and ... sometimes
people I'm working with, or students, they've got ...
all sorts of crazy indenting things that just ... I think it's potentially
extremely confusing ... and that the highlighting I think these
... the color-coding that you get in editors like RubyMine
and also you can get in simple editors like Vi; well Vi's not that simple, but
ASCII based editors like Vi and Emacs and so on
just makes it hugely hugely
easier to avoid these bugs. Writing the tests before you write the code
that's one of critical things I think
trying to ... asserting what it is that you want the code to do
... getting your assumptions out there ... doing it really properly test driven
... keeping it as absolutely simple as possible. Only ever writing
application code ... the smallest possible amount of adaptation code
in order to make your test pass is a great way of avoiding really nasty
complicated bugs. This ... I'm still surprised at how many people ...
given a homework instruction, an assignment or a project ...
in a distributed team, people just will say: "rights yes let's build the entire thing
let's let's let's
do coding coding coding coding ... reams of code
thousands of lines of code ...
Oh right then we'll start testing now." It's ... write ...
get down your assumption about what it is that you want to happen
in the simplest possible test that you can, make just that test pass
and then ... repeat, red, green and refactor
... so yeah one unit of functionality;
write the simplest code to get the code to green and then refactor ... I think that the complicated thing here
is nesting that within the higher cycle
the bigger cycle of the acceptance tests and maybe possibly even integration
tests
... there's sort of cycles within cycles there. There's like at the very top level working
what are you building for your
customer or your user base ... what's the highest level
acceptance test of what's going on ... and having that up there and being -
you're sort of bumping along at the bottom doing the individual unit tests
but sort of staying within that picture overall can save you
huge amounts of times in terms of avoiding bugs but one of the critical things of course is getting
help
... Dave and Armando come up with their lovely acronym R.A.S.P.
for their ordering. I'm actually ... I'm kind of a bit
.. I'd almost be like R.P.A.S or something. I think I tend to
advocate posting a little bit earlier in in the sequence in some ways
in that as much ... well
or least clearly you should be doing search. First off ...
reading the error message ... even though you're busy and don't have time;
kinda building up this intuition for understanding error messages is
... they're going to keep coming these error messages and the more intuition you
have about
how to deal with them the better ... absolutely ...
if there isn't an error message, let's go and find the error message it's there
in a log file somewhere
... so then Dave and Armando are like ... next it's A
ask a real person like ... if you're in an open plan office ... or
if you've got ... you might be in a Google Hangout with somebody, who knows?
... and you're in a pair programming this is the ...
ask a real person. I mean they're definitely ... that's certainly
... if you're pair programming and you're working on things together and an issue
comes up discuss that with the partner. That's exactly ...
if a bug comes up in a pair programming session that's ... discuss it with them.
That's what you should be doing right? You can also ask
in Skype chat or IM chat or whatever
else ... I guess sometimes the -
see partly why I ...
I put these here, you can just ask straight away in Skype chat.
In the case where you've got some error like this, rather than saying okay
you know taking that entire backtrace and then going over to Skype and
saying: "hey I got this back trace
and what's ... I got this error, analyse this for me"
is kind of a little bit you're sort of dumping a lot of stuff on people. If you can
take the time to read the error message
and see this is the thing why I would say do the search first; like so we take the
... we take the error message and do that search
... you can kind of almost save a ...
its ... particularly if you can find the load bearing part of the error message
you can save so much time of just okay ... I mean and then there's the second thing of like
well
can I interpret what's going on here ...
... the Stack Overflow I mean it's for ...
as you become a more experienced developer that's just ... you're going do that
anyway
... and we want to encourage I think students and junior developers to do
this
... as much as possible and start getting to know that
okay yes ... here this is like Heroku
... this is the Stack Overflow. These are the
organizations and the places on the web that are gonna allow us to
find the right stuff. Here we've got somebody else doing it in a
... community forum which is ...
probably gonna ... like or Google Group [INTAKE OF BREATH]
thats ... maybe that should be our second port of call or we look there if
there's only ... that's all there is because ... you really wanna be going
to ... what is it? This is a Heroku issue
when we've been deploying to Heroku in this case
or StackOverflow, always a good resource ...
and as the StackExchange for
edX 169 comes up maybe that will start appearing in the search results, so that will be good too
... but so ... with these kinds of errors
I would definitely advocate ... you might well search for them before
you ask
in the Skype chat and so then ...
Google's your friend, there's StackOverflow. Then it comes to
posting and I say ... sort of asking in IM
post ... if it's a really
... I would say if you -
you've been searching and not finding what's going on
and it's a relatively simple thing; it's like oh this is just not working and you're
in kind of like sort of a team, you're relatively
you know the team relatively well in your IM chat or Skype or whatever
... then you could just say: "oh guys I'm kind of sort of stuck on this
this thing ..." You haven't yet done a post. If it's like
... it's maybe out of the class context but if you're a junior developer and
you're
working on something and you've encountered a relatively gnarly ...
stack trace and there's lots of little different bits and pieces
and you're not sure ... it would be really good ... I guess it's sort of
... good manners ... maybe before ... it's a judgement call ... maybe before going on IM chat and just saying:
"I have this thing, or can help you with it?"
... doing the post to StackOverflow,
to a topic specific forum ... or in our case the class forum or what have you
and then pasting the link into the Skype chat so that's ...
you've kind of ... you've sort of showing people, doing people the courtesy of saying
rather just asking you to solve my problem; I'm showing you that I've kinda done
a fair (amount) of the work to understand what the problem is and provide a context and
so on
and put that out there and then post the ... and then that's out there
and then you post the link into the Skype chat and then maybe nobody's around
in the Skype
chat IM and doesn't respond, but then you've still ... you've already got
your thoughts and your thinking out and you've got a StackOverflow question out there
and ... while you're then doing something else that could get answered. So I
thinks that's
a reasonable strategy ...
... but for doing that posting, I mean it's
good manners
to read your error message,
have done some searching around ... this thing here it's yeah ... if you've got
someone there or you are in a pair programming session and you can asked them immediately then definitely do that.
You may be very isolated in which case ... fair enough you move to posting
a bit earlier
... yes StackOverflow's very good, read their guidelines
... I mean the critical thing and ... again in the textbook
there's great coverage of this but ...
so ... just saying "oh ... the sinatra gem doesn't work on
my system"
there's not enough information for anyone here to help you ... "The Sinatra
gem doesn't work on my system", attaches the 85 line error message
not so helpful again ... a bit more information. Best we've got this
...
actual transcript that's described in the book so
somebody is - here is - they're described what operating system they're on
... they're showing the sequence of things that they did
and they got this error. So this is ... this person here, Igor, has
really provided a good background on what he's trying to do.
You can see here within a very short amount of time
people are asking some clarifying questions
and I think within the hour ...
a precise solution was found and that's
... it's good, although as Dave and Armando point out
in the book ... you're not going to get instant response
on StackOverflow, it can be pretty fast.
... but ... it should be ...
you should exhaust the other options first
... definitely be polite I mean I think there's
the really easiest way to ensure that you don't get help
and ... that actually people start attacking you and you start
getting into sort of a flame war
is to be really angry in your post and say
oh this software is driving me insane ... ah it's this, it's this and ahh ...
I mean often we're in that mood where we're very frustrated when we're
writing these things up and we're getting stuck on them ... but to the extent that
we can be polite
and even if we ... it just, I don't know I think you're just much much more likely
to get a quick response to your problem if you're polite and civil
... and also sensitivity to the developers. I mean the developers are also human
... it's a bit like what happens in emails sometimes. We're kind of
there
and we say things maybe that we wouldn't say to people's faces because
we're sitting there facing the computer and similarly you know we have these
bugs come up from the -
from the system ... whether we ... they're user interface bugs or
software bugs or whatever ... there are human beings who are working to try and build
systems to do
different sort of stuff and as frustrated as we are with them;
it's important that we kind of, are sensitive to the fact that they've been putting a lot of
effort into building things;
just because ... the thing that they've built doesn't do quite what you want, or hasn't
worked for you
shouldn't be to completely undervalue their time
... even if they've made ... arguably they've made a mistake
at some point, they're still human and so sort of being sensitive to the
fact that they
are putting a lot of effort into creating very often the open source systems that
we're using ...
is going to go a long way towards ... endearing you towards the community
... but so going beyond sometimes as I sort of mentioned previously
I think sometimes
as much as we have
considered and thought over and we've posted on StackOverflow and the discussions
going on;
maybe sometimes you're not going to get the answer that you want
or in IM chat. Sometimes as I say video maybe worth a million words. Shall I coin that phrase,
is that my kind of trademark that and get some small amount of money every time some people say a
video is worth a million words?
Doing a screen share is the way to go and
we'll be strongly advocating students and TAs doing pair programming.
We'll be talking more about that very soon alright bye for now.
