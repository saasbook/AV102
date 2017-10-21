https://edge.edx.org/assets/courseware/v1/a99b113d97374b7c6bb5fb0554ecc584/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/3.4-_Pair_Programming.pdf

Yes, so let's talk about pair programming ... we have a
wonderful little image which seems to be all over the internet
... I think that the worst view of programming is that it's wasting
one person's time ... that other person here might be a cat
they're saying things like look look look you forgot a semicolon and it's like no we don't even need
semicolons or it's like yes I was just about to do that
it's you know the kind of ... in its - I guess what's the what's the word it
...
its monstrous form - it's argued to be
you know kind of a waste of time. I think that view is becoming
less and less prevalent. I'm a bit of a pair programming evangelist. I think it is the
way
... and but you know why should you listen to me?
We've built all of our AgileVentures
sites and web apps through religious
pair programming ... other companies like ThoughtWorks and PivotalLabs and so on
are just basically getting things done and having a lot more fun
doing pair programming. What do we mean by pair programming?
It's this style of programming, you
sit side by side at one computer; it's the remote ... well
not remote; it's pair programming; we're all about remote but anyway; pair programming just
by itself
and the idea is that rather than like one person staring off into space and the other
person doing all the work ...
and the other person occasionally getting coffee, it's that your continuously collaborating on
the same design,
algorithm, code or test ... and in particular that
it should be ... there should be a process of really tight
tight focus ... on the code
... and so why is pair programming useful?
One of the key things that it does is it really increases your focus level
... I think I find this all the time; I find myself when I'm soloing
which is when I'm coding by myself, which I hate,
... these days ... the tendency is to kinda like wander off and think about other
things
... with ... you start cutting corners on the tests or
... what have you; but by having another person there
... that can really keep you focused on the
on the problem. It can allow you to brainstorm
more effectively ... these things
kind of ... they will ...
if your pair is somebody who basically is a Facebook addict and can't stop looking at
Facebook and talking to you about Facebook
then that is going to be a problem ... if you're
pair is somebody who ... never says anything
then the brainstorming is not gonna leap up.
It's not going to suddenly be
better than it was with just yourself. So to a certain extent it depends on
the -
on the pair; all of this does ... but
that's partly why I think it's important for people to understand
how to do pair programming well, which we will be talking about in this section; particularly
remote programming which
gets round all those pesky: "oh he's in a different country and in a different time zone"
issues ... but so the other thing ... and for me as a project manager,
the thing that I *love* about pair programming is it's increasing our truck number.
Rather than having one huge feature that we're developing for
a customer
being done by one person and then that person accidentally goes under a truck and we have no
idea how the code works
... we have two people
working on ... at least two people you know and ideally
because we'll practice promiscuous pairing, like *continuously*
... three or four or five different people will have paired in different parts
of that code base on all of the
little technical tricks and skills that one person is discovering,
they are getting shared through the team and the knowledge about how to deal with
certain
libraries and gems and javascript things and what have you
is all being shared around;
that's extraordinarily valuable really from the point of view
of a project manager ... and the other thing, I mean, this is ...
I think, pretty much everybody wants to pair with somebody who is -
you know - at the same level as them, or maybe slightly above in terms of what they are thinking about
levels; whether it's level on JavaScript or level on
this that and the other. Personally I enjoy pairing with people of all different
levels
... sometimes it's a novice; someone who comes with fresh eyes
and sees what you're doing and asks
an important question, and you can say: "Oh right! Actually we don't need any
of all of that stuff, actually you've saved me three days work because you know you asked
that question
at the right time and personally I mean I'm a bit of an extrovert. I mean I guess if you just don't
like people,
then pairing is not for you;
but if like many other people you do quite like interacting with people and you also like
coding, then you can mix it together
and it can mean that coding can be a lot more fun than it can be - I think
particularly
because there's this thing that as programs I'm sure that we've all encountered
where something just doesn't work and it just ... you're just stuck
and being able to talk to somebody else about that at that moment when
you're stuck
rather than just you're searching StackOverflow and you're posting to the mailing lists and
so on
and you're like er er bang bang head on keyboard ...
actually going through that process with other people together is ...
makes it all the more manageable, yes
indeed. So what about the actual software that's coming out?
I think ultimately there's a number of statistics ... there has been a lot of
research done on the costs and benefits of pair programming
... it is obviously you're having two people do what conceivably is one
person's job ...
there is an increase in getting things working
but that's made up for because you just get ...
higher quality code ... that down the line there's less
... bugs to fix; there's less issues to address; actually it
reminds me something I was going to mention ... I mean you could say, "Right, about this
truck number,
ah yes, well if the person had written
fantastic documentation that explained exactly what they were doing
all the time that they were doing it
and they kept that documentation completely up to date then
we wouldn't need all this annoying pairing activity would we?"
... it just, it seems to me the danger even if
you're sort of religiously fevoured about documentation
... there's sometimes no substitute for
actually having experienced using something. This is why
fundamentally screen share is so ... I mean I can write a huge
long post in a forum to say look I'm having all of this issue and I'm
stuck here and this and the other
... a screenshot of
exactly what's going on, or indeed a live session where I'm talking and going backwards and
forwards for somebody
really cuts through; I mean extraordinarily so ...
such that ... I dunno I think in trying
... maybe in the ideal world people would work well independently and they
would like
document everything perfectly and thats I guess if you've got ...
if you're in the army and there's some
huge amount of money or a gun or something or whatever it says: "Right!
You must behave in this way!" But I think it's fighting against
people's tendency to just see if they can get something to work
right? ... I love documentation in the form of
executable documentation, that's what I want. I want my documentation to be
executable. As we
can then run it, and then it can go blue or green or blue, red. No; green or red
depending upon whether it's actually a reflection of what the system is doing!
Anyway but so I mean ...
the code you get out ... I think you just basically get better quality software
as a result of doing pair programming. The code is continuously reviewed by more
than one set of eyes
... mistakes get caught earlier and ultimately your
confidence in the code is higher ... I think
there's ... I mean I have this argument that goes backwards and forwards
... with people ... learn ... there's
... people dispute the ...
increases in the benefits that you get in ...
let's say the working world ... I think ...
in terms of learning coding ... Laurie Williams
led this research at the ...
University of North Carolina State demonstrating how much faster
people could learn when they're pairing. So even if you were like:
"So well, no, no it's just not going to be efficient for us!"
if you're learning something I really really recommend as there's a lot of evidence to suggest
just that you'll learn much faster
if you're doing it pairing. I also personally, I would really not
want to be a project manager
on a project where pairing was not sort of rigorously
enforced. Although ... there's continuous review -
you can be, as I think we'll talk about in the next section ... there's pull
requests and there's reviewing code after the fact which I think
also needs to happen; but I would much rather, as a project manager
reviewing code coming/being submitted to the projects,
I would much rather have two people having worked
on that. Two sets of eyeballs going back and forwards, before I then
lend my set of eyeballs ... to the finally submitted pull request but more on that
... in the next section ... so
again I mean the pair programming it's not this side by side you know one person
just half falling asleep ... there's this idea the driver and navigator
... and the driver will do - the typing and the navigator
... will be constantly reviewing the code and
thinking about the longer-term strategy and so on and talking
all the time. It's also important to switch roles ...
I think we talk about 15 minutes being a good switching time, but you need to work
out your own
... pace ... it's ...
pair programming is a skill ... we
piloted pair programming among students in
the MOOC the last time around. In 169 in fall 2013
and ... we had some very very positive reports and we have some negative
reports and there's
a big thing about your personality and
getting used to doing pair programming and so on ... so
we're working hard this time to talk more about
*how* you do effective pair programming. I think that's a whole skill
... what I often say to learners is
master the pair programming skill first because then every other skill that you
want to master like TDD or BDD
or writing a gem or whatever ...
if you've mastered the pair programming bit, everything else will be much much
easier
at least that's my opinion anyway ... but so there's this idea that ...
I mean in some ways this is soft
fluffy friendly skills that are not part of programming. Programming is all about
understanding
you know algorithms and logic and so on
and we're not talking about emotions a lot are we? with software. Actually in my
Software Engineering classes
I say that - really - programming is an emotional experience, even if you're doing it by
yourself
how you cope emotionally when you get stuck is
... I think that's ... how you deal with that; because it's a
very frustrating experience;
how you deal with that is a lot about who you're going to become as a coder and
whether you're gonna
succeed or fail in the programming market shall we say
... there's this phrase ego-less programming which is about trying to take the egos (out)
... rather than whenever anybody suggests something, you defend
yourself and you're "Well, ah no!" and then you make up reasons for why
I have to do this or have to that ... it's sort of trying to learn how to ...
accept
constructive criticism about ... saying right this is a collaborative
activity that we're doing
... we've got I guess I won't labour the point here we've got
... there's a variety of excellent videos by different
... shall we say, leaders in the field; far better programmers than I
... in the accordion navigation which of course is difficult to find. I'll highlight
thats
...in the intro to this section but ... yeah, so we've got various
videos ... targeted at different
levels ... you can hear from them about
you know the best ways to sort of approach things emotionally
... what I wanted to highlight, moving on from the emotional side of things,
is I think that pair programming is just
one type of collaboration with one kind of target
task. So this process of
switching driver/navigator roles is also, is
often called "ping pong" as in: tush, tush, tush you know the game like tennis but you
stand on a table, no no no anyway, you don't stand on the table you stand next to the table ...
I don't know ping pong very well, but this is ... I'm talking about pairing ping pong
and, oh I've jumped a slide ... let's go back.
This is one type of collaboration of
a number and partly as a result of you know the last year of
promiscuously programming with an extremely large number of people. I think the
number of people I've paired with is up to about 500
and climbing and also with working with you know
all the MOOC students and working with Hawaii Pacific University and also with
Makers Academy
in London, which is a coding bootcamp here;
I've started to develop this list of
different types of collaboration; particularly in terms of programming
but we're also doing it
in terms of other sorts of activities like you know developing course
materials
and so on ... developing advertising copy or what have you
... but so ping pong this process where it is very very tightly focused
backwards and forwards
you've got this master/robot thing where one person is just telling the other person what to do;
you've got scaffolding where you've got an expert who's working with ...
where there's sort of an extreme difference in expert and novice
and there's just sort of side-by-side programming where you are like ... are you
even working on the same task ... there's just having a chat, and then all of the different
set above with observers. So you could take any of these
and you could talk about them as a collaborative mode for programming.
And you could insert any other task; so if you take ping pong
and we say we're doing it with programming then I would say arguably that's sort of
true
pair programming in the Extreme Programming vision of what it
should be like
... let's consider that there ... so the ping pong versus
side by side ... I would describe the ping pong thing is your ping ponging
backwards and forwards and we'll
look at more details of how that might work in a minute; on a problem
where both parties haven't seen it previously, or at least not recently.
So - and I actually I put that in to distinguish it from the situation where
you know you might have ... you already know the solution and you're working with
somebody who doesn't know the solution to the problem
... I think ... true pairing really is ...
... well ... do we even really need the term "true pairing" ... I'm not
sure
but I think that the
almost the kind of ... it's kind of like free climbing ...
the ping pong where ... you're both working on
... something and you ... it's a new feature
... and you might have worked on things that are similar to it before, but this is the
new one
and we're doing this and its ... you're both
... you're not so enormously different in the terms of your skill
level or experience with
the technology, which let's say it's Rails or JavaScript or Jasmine or whatever it happens to be ...
and you're working on it together and you're basically taking turns to write code
backwards and forwards or taking turns on whatever the activity is. That's
really ping pong. It's really tight collaboration ...
you might have ... we can contrast that with side by side so
you may be in the same space, where that might be the same office, or it might be the same 
Hangout
... and you could be working on the same problem but you're both ...
you've both got access to it, but you're not actually kind of swapping backwards and forwards in a
ping pong when you're in the driver and navigator roles.
And so that's this sort of side-by-side activity and
that's something that you can do. I don't think it gives you all of the benefits that we're ...
I mean these benefits that we're talking about
... for pair programming here; and they come from
when you're doing this ping pong backwards and forwards in
tight succession
... I mean you can even have - it could just happen to be - it's like you know
open office -
we're side-by-side and we're working on a different problem but occasionally we
say things to each other like: "oh I'm sort of stuck on this thing" or
what have you ... and that's kind of handy to have other people around when you're working
maybe on the same problem or a different problem; but if you're kind of really ...
not ... if you're not in that sort of tight collaborative zone I don't think you're going to get
many of the benefits of pairing. Not that these things ... I mean
... it's actually quite nice to have somebody next to you
working on a different problem that you can occasionally say: "Ooh, you know, this thing, that thing"
and so on. That's a valuable thing and
in terms of thinking about managing distributed teams, enabling people ... like having a
Hangout
set up so that people can just sort of hang out there and work on independent problems and
occasionally chat to each other:
really useful ... I think you know we'll be doing that with the
Help Desk Hangouts for the 169 course but if you're thinking about managing your
distributed team,
just having a sort of continually running Hangout that allows them to kind of have
a sort of an open office space shall we say ...
but virtually setup, that's really really useful
... and going on to two other of these collaborative patterns like what I call
master/robot and scaffolding and these are particularly important
for ... I would say
anything in an educational situation because master/robot and scaffolding
are where we're sort of assuming that one person knows
the solution to the problem or they know the domain area
really rather a lot better than the other one. Now of course
that doesn't mean that person is somehow better across the board at
absolutely everything ... for example ...
we might be working in a Rails project and I might let's say
I have a relatively advanced Rails knowledge ... I don't compared to
many people but compared
to some people I've got a pretty good Rails knowledge, but let's say that I've got a dip and
I don't know Jasmine
testing quite so well and there might be somebody who's done a lot of Jasmine testing, but they don't necessarily
have
... Rails; so it's like
... this idea that people are kinda on this continuous scale
from super ninja programmer down to like programming novice
and that they're stacked up and it's like oh yes. The thing is that there's so many different
things that you can be expert in, in terms of the technology field ... in the
world, in life;
so everybody's got different levels in all of those ... they've got a different sort of profile in
all those different
domains; but anyway for the master and robot distinction
there's a thing that you can do, if you know
pretty much the prescribed recipe to get through a problem
you can just tell the other person what to do, you can say: "right, type this line of code in here
and save that file and do that thing and do that thing on that website"
and that's sort of done; and that may have some benefits to the person who's being
the relative novice
who's being the robot in that situation but I think it's not as helpful
as if you're set up with a sort of a scaffolding approach, and we've talked about educational
scaffolding
previously and that's as you know where one person knows the problem
solution; but rather than
just saying "do this and then do this and then do this" maybe with a little bit of explanation
that they actually scaffold the novice
in their attempts to "master the problem" hmm that's confusing;
let's have it "solve" - in their attempts to solve the problem this ... so
rather than giving them answers you say: "What do you think you might do in
this situation?"
and "Well, you know there's a couple of options here; there's this one and this one.
Which one sounds
good to you?" and this is I think the sort of true skill
of the ... is it the teaching assistant? Shall we call it the coach? The guide? The
instructor? What have you;
is kinda trying to manage the ...
stress load of the person that they're working
with - to say "you know okay I'm gonna give you this piece of information
here because
... I think that's you know just
you can just remember that later" but if there's some sort of key concept with
TDD or BDD or with Rails or MVC or whatever it happens to be
if you can rather than just giving the information; if you can scaffold
that person so that by giving you know little bits of help
you can help them find the solution; I think that's
hugely beneficial for ... the learner
in this case ... so and
... we're in this brave new world now where
you can jump in to a Google Hangout with anybody anywhere in the world and start helping
them
with another issue. I mean we had a remote pair programming session on Wednesday evening this
week
and there was a guy in Columbia showing me how do you use MeteorJS which I don't know very
much and I was ...
I think he was less familiar with git and GitHub than I was and I was ...
we were kind of like ...
we were doing scaffolding almost doing master/robot because
we were both so relatively inexperienced in each other's domain
... but we were still getting something out of it ... I mean I think the important thing is
is that ... I'm not trying to say
oh you must always do you know one particular version of these different
types of collaboration but it's to be aware that there are all these different types
and they're
made appropriate by what you're trying to achieve, what's going on
and so on and so forth; and then just to sort of round it out I wanted to mention task
focus chat and observers
so sometimes ... we're setting up a remote pair programming session. We want
to do ping pong
but then actually we end up spending all the time that was available
just chatting about the problem domain and that's
not the end of the world. That can be very useful ... but again it's good to
distinguish that from pair programming ... you might have like
chatting about the problem domain and you do a little bit of stuff on the
interactive terminal and you're exploring and it's not really this sort of focused
ping pong, but I would tend to call that task focused chat
and it can be very useful and I think to the extent that we have
words to describe all these different sorts of behaviours
that's handy; like going forwards for the - the MOOC course
then potentially you'll be sort of pairing or scaffolding pairing
... which is actually another topic I guess ... rather than scaffolding the individual, actually scaffolding
... a pair to help them do the pairing ...
... I'm hoping that we'll be able to talk about these sort of terms and we'll say "Oh
you know
I got a couple of students set up with pairing but they seem to go into just doing a sort
of master/robot thing" or
"Oh actually - you know - there's this guy - you know - from wherever
was doing some really great scaffolding perhaps we should promote him to being a
TA
on the course?" and so on and or "There's this other group
they just ... there was five of them and they just seemed to be doing side by side programming with
not much communication"
So having a terminology to explain
... to refer to these different types of behaviors and the different things that
people might do
... in the context of the MOOC is going to be online; I think it's going to be very
important and useful and then so finally
... all of those different things, we've got five different things there, any of those can happen with
some number of ... one or more observers
... who may occasionally ask questions ...
or may not, they may just be visible and I think
I mean the thing that we always do and talk about in AgileVentures is say that yes
just everybody observe!
Please observe! Don't feel that you have to get involved I think you know
people have all sorts of trepidation about getting involved in pair programming
about getting involved in online scrums or what have you ...
it's always fine to just start observing; that's our policy; and ...
you know we certainly encourage people to ask questions when they're ready ...
and that can be of value. Sometimes the questions can be valuable; it sort of promotes this
expert in earshot learning; if you can kind of sit and watch some other people
who relatively speaking are experts on doing something ... then
you can get a lot of benefit from that ... so
there we go. So I think that's - that's - all I wanted to say about the different types
of collaboration there. I just want to go now I think finally here
into some ping pong specifics and there's actually ... so we talked about ping pong and
pairing where we sort of swap the
driver navigator roles in relatively quick succession.
There's actually these sort of micro pairing things that are prescriptive
in terms of doing your
TDD or BDD ... I guess I
have mixed feelings about the TDD/BDD terms but Red, Green, Refactor is I
think something we can all
we can all relate to; and there's this idea ... I love this
... this is attributed to John Wilger who's I think one of the
coaches in the XP domain of how you can sort of mix in your
Red, Green and Refactor, which of course we're all doing, with the ping pong.
So the idea here is that we've got person A and person B.
So person A would write a failing test
watching it (fail) we always want our tests to fail of course because otherwise we don't know if they're working or not
... then person B would come in and say right I'm gonna fix your tests
I'm gonna do some refactoring. This is the driver navigator roles
swapping here from A to B. So A has initially been typing there to write that
first failing test. B has then
written some code that's made that go green ... B's then refactored it
... discussing that with A
quite likely and then B has written a test
of the next step as it were. Right, the next test to watch something fail
... and then it swaps back and depending upon the complexity of what you're
working on
... this might be two minutes or five minutes or twenty-five minutes and
and so on ... thats something else you've got to
take into the mix, but then you go back to A. The person then
makes it work they refactor it; write a test, watch it fail
and it goes backwards and forwards like that; so that basically rather than ... I mean
you could have a situation where
one person wrote all the tests and the other person made them pass which is kind of
... in order to get kind of a nice balance between
the kinds of demands that the two pairs ... the the two people in the pair
are making on each other; you've got this framework for pushing it backwards and
forwards
and we've got some videos of myself and other AgileVentures
people doing ping pong on some - on some Kata
as a specific example of how that works ... and thats ... I think thats really useful
to kind of have
... partly to kind of avoid arguments about
... when it's time to swap the driver/observer role ... the driver/
navigator role, I should say.
I mean the danger is that you start off doing ping pong
and it descends into a kind of side by side where
the driver won't give up the keyboard and so the
navigator drifts off; stops thinking about the same problem, moves on to a different
problem
and they're just working side by side and that's not really
... I think there's some benefit from that but nothing like what you get from
a really tight ping pong on a problem
... and if that were not enough as I mentioned there's other ones
and there's a fantastic talk by Sam Livingston Gray which goes through these,
we've got linked in, but they're so good I've pulled out the diagrams ... I think they're fantastic
is
... there's this "change the message" so this is
... particularly if you're working in unfamiliar code territory
where
this kind of loop would take quite a long time, like maybe half an hour to get ... work
through all the different error messages;
another way to do is to write a test and watch it fail and then
... the next person rather than taking it all the way through going
green as you swi(tch), as the next person ... there's a person B becoming the driver
they would just change the message ...
maybe it's a different kind of error message ... the test is
still not failing for the right reason
and so you might go backwards and forwards ... adding a few bits and pieces
... changing the message each time and that's particularly useful I think when
you're
both exploring a relatively new library or new technology
or what have you and ... it can then ...
the interesting thing is once you've ... as a fairer, once you've got this idea of
right, make it work
change the message and then we've got this other one called "One Undermanship"
Once you've got that down you're kind of saying to each other "Ooh you know
this seems to be taking rather a long time" ... you might be working on this
and you've
planned to - to make it work and so you say: "This is taking rather a long time you know shall we
switch to
you know I've got an interesting error message here; do you want to try and change the
message?" And person
B will say: "Oh yeah no okay that's good lets do that" and so
depending upon how long things are taking you can switch backwards and forwards between
"change the message" and "make it work" and so on and then there's also "One 
Undermanship" which is kind of
where you purposely kind of ...
expose ... well it's interesting ... you sort of purposefully expose flaws
in the person's test suite. So for example here this is just with
a trivial
code example here but so you ... somebody does one sort
of test case and you basically rather than actually
... you sort of pretend almost like you're a computer ... a
robot
and you do the absolute minimum effort in order to get the thing to pass
ignoring the intention that might be ... in there, in the ...
the method definition or in the name of the method. So here
with this test, this person who's swapped over, they're doing kind of "make it
work"
but instead of kind of saying this should be generic add
you sort of hard code the solution ... and then you don't do any refactoring and you say
"ahaha" and you add another test and then so here we've got the ...
goes back to the driver becomes ... person A becomes the
driver again
and so now ... again rather than completely solving it, you only partially
solve ... with a bit of hard coding
or just enough to ... what the absolute minimum amount that would make
the existing tests
pass and then ... add in your next test and this is
... it's sort of ... you can see this is a trivial sort of game with this
particular code
but this is a great way of making sure that the tests are really testing
for what's going on. And then there's sort of a judgement call there, about where
do you
draw the line ... because you could keep on
writing, hard coding, you could add like a dictionary with lookups that says
right I'm gonna look up only exactly the test cases that you have
but I find this is sometimes a useful strategy
to try and force yourselves into getting more rigor in your tests
but again the ... I think the critical thing is to kind of understand
these terms and be able to use them as referring to your
pairing activity ... and so we've got video ... I think we've got videos
that include elements of all of these available in the selection; we've got more people
talking about
pair programming ... just to link this back up to distributed teams;
I think this is the other thing, it is for team coherence ...
at the bigger level if people are pairing with each other ...
whether they are in a team that's working on software for the space
shuttle or whether they're
students collaborating in order to try and learn; whether they're doing that in a bricks
and mortar university,
they're doing an online course for a bricks and mortar university; they're doing it in a
MOOC or what have you
that process of having people connect and communicate ...
with each other is extraordinarily valuable for the outcomes for everybody
and it's just ... I can't emphasize it enough ...
... whether you're sprint retrospective
meetings are two hours or three hours I think is far less important than
the fact that you've got your team
really communicating with each other and pair programming ...
of the ping pong style I feel ...
fundamentally engages people and forces communication in a way that's really really
good for
the team, it's really good for learning, and I just I'm a bit of an evangelist
... that's not to say that pairing doesn't go wrong sometimes
its ... like communications with - with any
people can do - and I think thats where it comes back to this sort of
emotional situation of how to cope with
your partner ... how to deal with egos
and I would say that the key thing there is rather than saying "Oh, pair programming
works or it doesn't work"
I think the key thing to say is that, if any individual becomes
skilled at pairing they can, like me, go and meet people around the world and have a
lot of fun doing it
and it's about learning that skill of pairing; and I can't emphasise this enough:
you learn that skill of pairing remote or otherwise, you get that down and
suddenly you've got a huge acceleration on how fast you can learn absolutely anything else.
So if you get this one down first ... again another analogy
I compare it to TDD, Test Driven Development
is yes, it's painful overhead at the beginning
to get it right - to get TDD - and it seems like it doesn't make sense and so on
but that short-term pain leads to huge long-term gain and I think that
the software world is coming around saying yes we really need it.
I would say the same of pair programming; there is potentially
short-term pain; for me not very much but ... there is potentially
short-term pain, occasionally there's pain that comes up; but that short-term pain on pair programming
can lead to huge huge long-term gain as I think
nicely evidenced by what we've manage to achieve so far with AgileVentures.
So I'm looking forward to lots of pair programming going on
in the MOOC ... having lots of fun
with the different ping pong mechanisms and maybe I'll get to pair program with you
before too long? Alright, bye for now.
