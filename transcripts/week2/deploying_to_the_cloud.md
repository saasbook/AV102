<a href=https://edge.edx.org/assets/courseware/v1/2d7e7454c6204a931264631c4b2cfb7a/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/2.5-_Heroku_introduction.pdf>Lecture Slides</a>

Hey so let's talk about deploying to the cloud. The cloud!
... I'm not sure if I like the term cloud ... it's used a lot these days
we mean stuff out there, in the internets, in the interwebs ...
there are also these two mnemonics I-a-a-S
and P-a-a-S or Infrastructure-as-a-Service and Platform-as-a-Service
that are really, they are changing the game
and they're changing not just the way that people get their software
out there and get them to their customers but also how teams
collaborate ... what's happening is that it's
you know becoming less and less ... common to have your own
you know - server boxes in your office - actual computer's running in your office that
host your code. I can remember back in the day when that was
you know that was often how it was you know the servers might be a in data center but you'd
sort of
... you'd have physical access to them
and that was sort of the norm when you wanted to get some sort of service
make it available to people you know on the web ...
or on the internet. You know there are now various companies that offer
hosting at different levels of granularity ...
you've probably heard these terms as a result of taking the 169 course before
... Dave and Armando have talked about that ... Infrastructure-as-a-Service ...
a good example of that would be Amazon Web Services which you may well have you may
well have done
all of the assignments for the 169 course
on an EC2 instance .. with Amazon ...
... and then very likely you will have deployed ...
applications to a Platform-as-a-Service such as such as ... Heroku
but yeah, let's talk a little bit more about the differences between
these two or how they fit into the bigger picture. There are all these
different kinds of cloud service models
great diagram here that's available on Wikipedia also a great article there
that you can read about the differences between these different things
we're going to concern ourselves today with Platform-as-a-Service
and Infrastructure-as-a-Service. In fact particularly focusing on platform as a
service
and Heroku which is one example of that in particular
which of course many of you will be familiar with already but it's you know great to have a
refresher on these things ...
one: because it's so useful for distributed teams and also because ... I
think it's a key sticking point
for students ... in the 169 Engineering Software as a Service course
... you can also see we've got, have I got the Kindle edition
here ... it's chapter 12 in the the latest in the new
1.0 edition has got ...
you know - an overview of this Platform-as-a-Service, Infrastructure-as-a-Service
and various other good stuff. So do ... y'know have a read you know
reading that chapter ... certainly the beginning of that chapter will go well with - 
this week's - this week's work ... but it's really about
... I guess the kind of how low-level access
you're you're getting. Infrastructure-as-a-Service gives you more access to the
underlying system and then gradually you get less and less as we go up this
stack but let's let's talk more about that Infrastructure-as-a-Service
or IaaS ... so as admittedly the key
difference now is that you don't have access to the hardware, you can't
phone up Amazon and say I would like to go and see my server. I mean maybe you can but they will say
"No, that's not really part of the deal"
what they're offering is you know ... some virtual machine
on to which you can deploy things .. not just deploy
code but you can actually - you know - choose as many of you I am sure know
you can choose which operating system you want to put - to put in there and
you know that's up to you ... to get what you want on it to do what it wants
but you know keeping it running keeping it you know fed with power and keeping it at the right
temperature
you know all the sort of physical things that's now the service that something
like Amazon
is - is providing and then often you know these Infrastructure-as-a-Service
will provides lot of things that you would otherwise have to be bothered with
which is sort of like back up of the system
... securities, firewalls, load balancing - all ... different stuff. You know getting the
actually the rights to the software - and so on and so forth and
so forth ... and so this is - you know - very convenient
... Dave has got you know wonderful examples talking talking about
... I forget is it with the FarmVille folks
... you know scaling their ... you know scaling through their enormous growth
at the beginning using just a credit card account with ... with Amazon
so that's - you know - Infrastructure-as-a-Service ...
not critical I guess to - to understand
Infrastructure-as-a-Service in order to ...
you know make it through the 169 a Engineering Software as a Service course
... you know if you are using an EC2 instance to - to - to run your version of the
virtual machine
then yes - that's that's very important but actually you can kind of
not worry about it too much. From a distributed team point of view it's very important to
understand
the difference between ... using something like EC2 or something like Heroku
and how - there - you know which ... you know how you should be making a choice between
those ... those two alternatives ... but the key thing really is the Infrastructure-as-a-Service
you've got
low-level access you can kind of choose your OS and you can you pretty much y'know
build anything you want on there. So there's a lot of flexibility ...
but that does mean you know a fair more bit of work.
Another alternative is going up another level of abstraction shall we say
is to go to Platform-as-a-Service ... like like Heroku or Ninefold or someone
like that
AppFog I think is another one and so this one it's its the Platform-as-a-Service is kind of built on
the Infrastructure-as-a-Service ... but what it critically has it now they've
made a decision
for you ... about what the operating system is gonna be
likely what the database is going to be ... you may have some control over the Runtime
Environment
... you - you know - and framework but there may be restrictions on which frameworks
are available; whether you can use ... Sinatra or Django or Rails or all these
different
- you know - different - different things but so as
many of you will be familiar with from Heroku or other Platform-as-a-Service
... you are not at ... you know when you're going into it you are not saying - right - I want to
choose to have a Ubuntu or I want to choose to have
... you know windows or what have you. You're saying - right - 
... I've got an app that I've made you know in Rails
... is of course the classic one that we did in Engineering Software as a Service
and then - all - you know - as well as - as we had in IaaS - as well as you not having to worry
so much about
the hardware, load balancing, firewalls, security. Although - you know - still -
you need to be aware of - you can still, you know, encounter problems at
... the higher-level but at a lower-level you don't have to worry about those and
now in principle with Platform-as-a-Service you don't have to worry about
you know - uh - what was the operating system what was the database. I mean -
you know - it's sort of set up for you you don't have to set up your own Postgres
database ... Heroku will do it for you.
We've got a nice diagram here from Franky Boucher
... which we've replicated
I think it shows you kinda on one side on the left side here
we're got Infrastructure-as-a-Service where you need to decide on these things on the top of
the stack the middleware, the runtime, the database
... but the lower level thing here the operating system, virtualization,
... servers, storage and networking is kind of managed by the
provider. You may have, be able to choose which operating system you want but they're
you know saying what's gonna be available for you and you can see here 'cause of
quite clearly because if we look on the
right hand side; is it left right? I always get confused my left and right, but anyway ... yeah blue side
left side, Infrastructure-as-a-Service. On the right side got Platform as a
Service.
So now decisions about the database and the runtime and the middleware
are now managed by the provider and you
really deal with the data and the applications. So
... the advantages of this are that you can focus
uh - 100%; maybe should we ... maybe we should say - like - mainly
on your application code; because you do have to start being aware of -
you know - issues that affect ... you can focus more
let's say that we could focus more on your application code ... rather than on the on
the lower-level
issues - but what is fantastic is that you can
scale up and down the amount of resources that are available to that - to the extent that you've
got ...
that you can afford to pay for it - and there are other lots of ...
infrastructure components that you can add in. This is I think one of the really nice
things about
about Heroku for your apps is you can add support for additional backups for ...
email
connections for all sorts of things ... you know for extra logging and this that and
the other
and there's sort of a plug-and-play you know you need to get set up with let's say New
Relic logging
... sorry ... New Relic monitoring you know you can do that
relatively easily because it's it's already provided
in the framework, if you want to switch it on. So let's get a bit more
into Heroku. Many of you will already be familiar with Heroku I think they're
one of the most venerable Platform-as-a-Service
... groups. Advantages ...
of them are you know all the advantages that you'd expect
from using Platform-as-a-Service I think one of the things that I particularly like is
... the ability to
deploy those apps using git ...
and that just, you know, makes a lot of sense - you know you've got your
versioning system which is saying - right, this is exactly, this is the code
that's working! This it the working code! Right let's have that code, let's have the working
code
on the server running in production for the for the clients ...
but it does have, so and you know you can do git from the command line. You can also do quite - there's a lot of
stuff you can do
through the user interface for Heroku
and you know and then many things are also accessible both through the
command line interface
and the the graphical user interface and we'll see some
examples of that shortly but first let's talk about some of the constraints
... although ... it the deployment is dead
dead simple ... I mean although arguably there are even some services that are even simpler than
Heroku ... and the - you know -
there's easy scaling. The constraints really is the sort of section is that
there's a certain amount of things that you get for free
and, you know, what - as long as you're staying within that free tier
... you know that's that's a great playground for working out what you want
to do
... seeing if you're kind of prototypical system that you've built is
is working for the customer base for the user base that you imagine
... but so once you start to move out of that and you want - 
you know - logging that goes back further; you want ... you know, more bandwidth, you
need a bigger database and so on
then you are you are going to need ... to start paying some money but ...
it's a usually, you know, getting started is gonna be a while
before you hit those limits and you can have established ...
you know - if your ... if anybody is actually interested in what your - in what you're offering
before you - before you hit them ... so they, I mean, they have this web based tool, let's just
show you
actually my, you know this - this is my Heroku dashboard ... I as a result of
y'know doing lots of example deploys for lots of people I have you know all of these
different
example apps here ... what were we going to talk about here we're gonna
... I mean there's you know you can it's - it's - it's a nice interface to manage
things through
you can create new apps from there. I'm more often do that from the command line
... and ... yeah ... have
I got ... I guess if we go into - let's see -
the AgileVentures ... organisations there. We've got some of our develop
... websites - I don't know how much we've got but we can have a look at the app
... but you can see here for example -  I mean you get
the Postgres ... you know out of the box so to speak but
we've added here the paper trail, so that's a logging app and you can see
you know all of the Add-Ons for Heroku
you know you get they have free tiers and then they have you know, if you wanna
get more and more functionality
you can you know pay. So if we click on here and say get Add-Ons
we can look for ... you know there's a huge huge load of different Add-Ons
that you can used to do just about just about anything really
and and this you know the the ability to sort of plug-and-play
with all the different bits and pieces the things that you that you need - from
backups
... you know through the extra kind of search thing ...
we've got ... I haven't even really scraped
the surface. There's about ... five or ten Add-Ons that we regularly use
... in AgileVentures, but ... being able to
y'know access that in this fashion is - is very very very powerful
... yeah and and so I guess particularly as regards
... teams; I mean whether you're a centralized team or a distributed team
then the ability to manage your organization through through Heroku
so we have our AgileVentures one
here ... very very handy you can have have - you know
give the the team of people access to it but I think particularly
... while this is this is very useful for the centralized team it's
extraordinarily useful
for the distributed team ... who are not in the the same office. I mean
back in the day - you know a distributed - if the
you know - if you were relying upon physical access to
the server which was in one place that was very difficult you would have to
have some person there
now because we've got a Platform-as-a-Service like Heroku
a distributed team like AgileVentures can - 
you know we can give everybody you know necessarily who needs it
access to this team thing. They can be all-round anywhere in the world as long as they've got an internet connection
and they can get in here and be saying oh right we need - we want to try out this
additional add-on
we wanna do this we wanna do that ... it really suddenly
makes the distributed team ... much more powerful
... and then I mean the flip side of that is you know by, rather than
relying upon being in the same office to look over at your colleague's computer and he
shows you all this is
is working here the process of actually deploying
to the to the cloud means that you know you have a endpoint
URL that all of your team can look at and they can look at it everywhere in the world. So that's an
actually all of your customers, your potential customers and user testing, it's well, I'm getting ahead of myself as
I often
do ... but yes ... it's the kind of thing
all of you will I think be familiar with Heroku to a degree because there were
... you know ... there were assignments in the
169 course that involved deployment to Heroku but you may have only
done it through the command line, you
you may not have spent much time exploring the dashboard and the support for
organizations and this that and the other - but there's really is a lot there
... and very powerful ... and of course not just with Heroku
but there's many other ...
good organizations providing a similar Platform as a
... service ...
offerings and you know they're all busy competing with each other to
make the best offering but so the other thing that we can do is we can use
the command-line
interface to you know create applications we can see
that I've busily had lotsa fun creating I mean I need to go through and clear these out
but very very ... it's so easy and perhaps too easy
to create and rename your apps
you can take backups, you can configure the add-ons from the ...
database
... and you can also get an interactive shell
into your application as I think you may have seen in the ...
169 course but so you know if you if you haven't signed up for
Heroku, it's free, you know ... that's a great way to get started
I guess what I'm gonna do is just run through ...
kinda I guess outside the context of 169 I mean - you know - this - you may already be
familiar with this
... let's let's just see how relatively straightforward it all is
to get a little quick Ruby on Rails app ... up
onto ... onto Heroku ... and then also
talk about some of the common issues that can come up, the blockages, I think particularly that
effect
... students and so on but I've got what've I got going here, I've got
... I've got a little, I'm in my little directory here
so let's have "rails new" and shall we call it let's call this
... this ... managing distributed teams
MDT; managing distributed teams app so there
and we're going to get our little rails app created. You can you can do this I mean
in some ways arguably doing this with ... sinatra is a more straightforward and then we'll go and do
the bundle install in the background. Hopefully my network connection is fast enough
to make that ... not too ...
cumbersome. So let's just sort of talk about the other things that we're going to be doing. What I would do next
is I would ... jump into my app directory make sure that the
Heroku Gem is installed and then - this is the kind of key thing
is about - we would use git to deploy into the - into the cloud
and ... probably through doing the 169 course you've sort of become - 
sort of approximately familiar with this - but I think this is one of the most
fascinating things. Actually the the best
I shall just go and grab the diagram; this is the the Coursera Startup Engineering
... course had a fantastic diagram which I think is yet to be matched in the
diagrams that I've seen
that show the relationship - actually here between this is
Infrastructure-as-a-Service, Platform-as-a-Service and and git and so on.
And so ... specifically in the
Startup Engineering course on Coursera which I highly recommend by the way
... they were sort of specifying - you know -
everyone should use the EC2. They didn't distribute a virtual machine
in quite the same way ... but so this model would be if you were working
on EC2 for the 169 course this will be the same sort of set up. So you have
your
personal laptop your SSH-ing into
the box that you have in the cloud from Amazon
and, you know, so you're interacting with that remotely
and then you're, you know, developing some code you're pushing it to GitHub and
storing it and or pulling it back as necessary
... once you've got it working you know on your
Infrastructure-as-a-Service, Amazon EC2 box you could then push it to Heroku
... using git again and it ends up you know at some end point that you're
user can - can browse to ... the
situation if you are actually doing things on the machine as I'm gonna do them directly
now myself then you know the Amazon Infrastructure-as-a-Service
component is not there and this diagram becomes a little
simpler. I still think this is one of the best diagrams that I've seen so far and
maybe one day we'll work out how to make great diagrams like that; but
let's go and see what's happening over here so we've got all of our ...
all of our libraries have been installed with bundle now
if we're gonna go into managing distributed teams. We've got our new managing distributed teams
app ... lets do gem install
heroku. I don't know that that's actually a critical
thing here that we need to have it; but we certainly do need to do ...
I'll put that into the background there for the moment ...
- did that, did you not like being put in the background?
background
mmm - we'll see what happens there. Let's
do "git init" there ... and
yeah, we'll just add there you go, you see it's got the gem installed there
... I think I had it already weee!
things are happening in the background wohoo okay all right
so git and then I'm going to do add dot that's - that's
you can see the command there - so we're going to git add stuff; let's look at
git status
and see what's going on again, and is there lots of things going on?
all rights so we've got you know all the files because we want to be somewhat
selective
about which files we were putting in for a Rails app but just in the interest of
speed lets ... just get this
going as "git commit
minus m ... initial commit
so I've just created a little Rails app there ...
now we could go ahead and I guess the idea
is to generate a little scaffold we've got here from the Rails command line you can
generate things. Let's imagine, oh I don't know
the ... let's imagine that we ... you know we just sort of create a very simple
a simple app so this ... scaffolding will create the views and the
templates and this that and the other for us
... I guess shall I just use the example of the high score? I'm kind of struggling with ooh I should
make something up, something relevant to managing distributed teams, but imagine that it's a
high score for
you know let's call it for the team; it's a the high score; there you go, let's
have team there
So by generating the scaffold ... we're gonna put
you know a lot of little bits and pieces that we need in place
we can ... just locally if I do rake
db:migrate
let's see if it will just sort that out for me? Yep so we've got a little something in there, and
if I do "rails s" then, and this is gonna be very familiar
... well at least you may not have seen the scaffold but if we now just go to
localhost three thousand and what did we do, did we call it?
team? Are we now going to have a teams thing there? There we go oops
we haven't got oh what are they called? ah, they are called high scores okay ...
high scores like so
and there we go so you have a new high score or team and they are called
the west coast team and they have a score of 100 and
create high score and now we have some
scores. So you know the scaffold's rather boring but it's got you know basic
functionality in there for a Rails app I think it's always ... I mean some people don't like
the scaffolding. Is it too much magic?
I always think that was an exciting part of rails - that you could do that
but so now ... what we can do here is we can ...
"heroku create" and I will add to my
ever-increasing list of random Heroku
things. So we've created this one "gentle-beach-2829" like so
... and then if we follow on ... I could have given it a special name but I didn't
... let's try "git push heroku master" ...
although of course - and I guess I should mention here; so there's
often a place where people get tripped up is one: is getting the SSH keys set up
to communicate with Heroku. I've got them already set up here on my OSX environment
... that's just ... you know ... it's an area where you may well find in the 169 course
that a lot of the students get
get stuck ... understanding what's going on there ... we've got ...
you know an assignment this week
to help you - you know  work through that's that's just - you know -
... when this is set up correctly it can be incredibly smooth.
If it's not set up correctly and you don't have the SSH keys installed and so on
it can be a real pain. It could be a real pain ... but so
... another thing that ... I think is sort of fundamentally confusing here
is so for example here I've created this app; I might be tempted now to do "git push
heroku master" like so but ... if we look if we quickly to a "git status"
we'll see that actually all these parts of the scaffold ...
won't have been ... to be ... are not in my
local git repository and so this is kind of absolutely key here
we need to do ... you know get this
... scaffold in there. So if I do "git commit -m" and
added scaffold like so ... put that in there
... you know now this is going to be ... I'm going to actually deploy
code that I have working on my system into the cloud ... so if we now
try "git remote -v" we can see it's
connected up the key ... the heroku to
... gentle beach there and if I do git push
heroku master. Notice that I'm not using GitHub here at all. I'm just using my local git
repository
and ... using it to communicate with Heroku there ...
you could be also pushing it to GitHub but that's a that's another
thing. If we just go back to this
... diagram here. So in the simplest sense -
you know - this side of the diagram over here - can I do it? I can't really select this in the way that I want.
But ... the actually you can see in the background there that it is pushing up that little
Rails app for me ... in in the simplest version
I'm just going from the laptop here and I'm pushing my code to Heroku and I
haven't even bothered with GitHub
... and then that is gonna you know create an end point
of an app that people can get to ... and so oh we didn't, oh no no
... we've failed. Okay ...
actually it's one of the reasons why ... going with a
Sinatra app is easier than going with the Rails app ...
I've forgotten to do a couple of simple things which are
... all mentioned in the appendix in in the textbook
but ... you need to make ... well because Heroku
is using a Postgres database instead of SQLite we need to
adjust our gem file so that SQLite is
in the test and development groups and we've got our Postgres gem
installed and then there's also ... we need to you know
for the recent stuff on Rails on Heroku
we need to set initialize_on_precompile equal to false
and so but these are the kinds of things that can can really ...
trip people up its you know and
for me I do most of my com ... I'm more often
pushing to Heroku with an existing project that all these things are set in rather than doing it with
a
completely new one ... but so having set those things and of course
again ... having adjusted the app so that
... I have checked all those changes into my local git repository
I can then successfully push to Heroku - which I've -
which I've done ... but then even having done so and if I ...
go and grab in the URL that we've got that
on we can still run into problems ... like here you'll often see this
"we're sorry
but something went wrong" but that's to illustrate - you know - then
we can run our ... the commands from the command line to do the things that we need, for
example
like if we were to do there "heroku run rake db: migrate"
... I guess I should have showed you that Heroku logs their
... showing - you know ...
and this is one of the key things that's challenging for
people maybe not necessarily familiar with ... Platform-as-a-Service and so on
... is the difference between running the integrations on their local machine
and running migrations in the cloud ... anyway
hopefully this is a refresher for many of you there
but so now if we go over to here to our remote
system now we have high scores here and we could say
team, I don't know, let's say East Coast and give you a score of 100
as well and there we go we now have our Rails app
running in the cloud. So - you know - it ... like with everything
you know - just so it can be as easy as that! Often you know
even for a relatively experienced Heroku user you can run
run into issues with a new app
but particularly for people coming in and you know
encountering this stuff for the first time I think
you know a good conceptual understanding of the difference between
you know your software running on the cloud and the software running on your local computer
absolutely essential; and we'll have some
assignments that hopefully will help with that
... and then there's other things so you know the
something that can trip people up as a security issue is that you might
you want to be using API keys for a service and so on and other secure things.
The temptation is, initially right, so we're deploying everything via git, we need to sort of put that into
GitHub and so on ooh I don't know what's going on there
... there's an extensive config framework to allow you to set
just those ... keys that are necessary in production and so on and so forth
but that's just sort of scratching the surface there. It really is the tip of the
iceberg
... Heroku and Ninefold and other systems like them are very powerful platforms
and you know it's sort of through the 169 course you may have
only pushed to Heroku once or twice and you know it's not something you necessarily got
very familiar with
but ... you know ... as a TA for the 169
Engineering Software as a Service absolutely
you know to getting that really solid, like, what's going on with Heroku; you
know
the ... all the differences you know really helpful because it's kind of something that I
think many of the
students get can get stuck on. As a developer it's extraordinarily useful
you know, particularly in a distributed team where you can't just sort of show the person
sitting next to you oh look I've made this new interface.
By deploying it to Heroku you can you then get a URL
you can immediately ... share that
with whoever you know ... and that's just
getting feedback on the thing that you've developed is absolutely key. So
... you know ... and it's not so much that you
are leaving ... I mean ... well I'll say in our AgileVentures projects you know often the
person deploying to
Heroku will be kind of the team leader ... so you know absolutely essential that the team
leader's got
good skills there. They're being the person who's the
... as it were the guardian to see right all of the different
developer submissions they're going through and they're going to go into production right now
y'know make sure that they actually get up there on to Heroku ...
but the individual developers you know if they want to ... even if they are not
necessarily involved
in day-to-day with that process - they can be putting
the - you know - spikes that they do ... we'll talk about those next ... you know features that
they worked on, user stories
put those up onto their own Heroku instances and share that with the rest the
team
and - you know wherever they are world they can go and look at them and get
feedback on
and so on and so forth. So ... yeah I hope this ...
you know ... encourages you to try out Platform-as-a-Service
... like Heroku if you haven't. If you aren't using it all day everyday anyway, and in
which case you know
... thank you for taking the time to listen
... but do think I even if you are using it all day every day
I think that the you know the supporting other team members who are not using
so frequently or supporting students who are trying to learn about it
kind of ... this ... the conceptual toolkit ... and thinking about where people get stuck
with - you know - getting the SSH keys set up
and understanding the relationship between git, Heroku and GitHub and all the little pieces
that's you know a clear understanding of that will help you help others
Alright
