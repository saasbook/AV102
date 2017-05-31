<a href=https://edge.edx.org/assets/courseware/v1/efd182fa200b2b8f7a6c588f16f40b4c/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/2.4-_Version_control_systems_-_introduction_.pdf>Lecture Slides</a>

Right so let's talk about version control. You're probably not asking
what is version control ... because you're likely familiar with it already.
But just, just in case ... its - the idea is that ...
it's a system that records changes to your files over time
and ... this this can be ... I think that the tricky concept
for people who have not been too familiar with version control before even
actually the file system itself, just the idea that there are
you know files and that they are laid out in a certain structure and you can access them through the
command line
is ... potentially it's just ... you know something that
more experienced developers can take for granted that everyone understands you
know ...
file system, version control ... and so on but particularly if
you've kind of worked, you know, in an IDE
for most of your programming experience ... you know ... worked on individual projects
where you haven't used version control
... it's ... it is a new concept for - for some people and we need to remember that
... it's also absolutely critical for teams
really ... for collaborating whether you're - you're centralized or
or distributed but anyhow the key thing that the version control allows is
you can take individual files or in you know
the entire project's collection of files and different directories and you can revert them to
a previous state.
So I often like to describe it as a kind of - it's like a a checkpoint
in a game, in a computer game where okay right whatever happens afterwards, where you know
whatever
... kind of death I suffer at the hands of oh I don't know
like pogo stick ... pogo-ing snakes wielding ray-guns
then I can get back to this this earlier point I won't have to redo the
earlier -
earlier work. So being able to get back to that point, it's like having a time machine,
it's fantastic ...
you can compare the changes that you made as we
I think we've - as programmers - we've all experienced that
you know several hours lost to you know a small
... a very very very small punctuation issue somewhere in our code
... being you know with with if you've got ...
version control and you have snapshots of - you know - the working system and the
system
where it's broken you can do a - you know - comparison and highlight just exactly
what those changes are. So it's a
very useful ... you also get views of who modified the source
in the past. Again particularly if you're in a team and we're saying why was that thing inserted
head and the code that causes the production servers to explode!?!
... no - "no-one knows; sorry - oh let's do - let's have a look and see" oh yes well
you know Bert you shouldn't have you know added that
you know ... rm -rf system call and so on anyway ...
but yeah it really version control still very useful
in individual products still use it in individual projects but absolutely huge
for multiple developers and has been for a long time ...
it's ... like you know there are a lot of other ways of sharing
files like you know by sending them by email or using FTP
or what have you ... the idea with most version control systems is that you've got
... a repository where you grab that entire copy of everything
... and so you've got everything that's going on rather than sharing individual -
individual - individual files anyhow there are many types available
... Armando and Dave did talk about several of them in the ...
the 169 course ... we focus on Git here because ...
although I guess Git ... the interesting thing about 169 Engineering Software as a Service course
is that you don't critically need that much understanding
of Git you don't have to use it for the majority of the
the assignments you kind of, you're encouraged to do so
it has to be - you know - it has to be used ...
for - you know - to deploy to Heroku as we'll talk about in the next section
... but even then you can get away with - with -
with remarkably few ... commands but actually once you start
working with a - with a team on any significant project then having
really really good ... version control skills is
absolutely essential and we'll focus on Git
partly because you know it's what we use on AgileVentures it's what
I think now just almost everybody's using it's a
it is just so so good for ...
you know people working independently of each other know. Now why is it called Git
... Git; I am British and I can confirm that it does mean
that you're stupid, if you're being called a git. Thats
Linus Torvalds who is not British but ... I guess - you know -
grabbing our slang ... and absolutely - welcome to it welcome to it
... Linus who'd previously created
... Linux which is obviously a great thing and so much of the web and the internet
runs on that
... what should I say ... much of the things that are running on the internet computers that
are running Linux
... internet and web: do you know the difference? can you? answers on a postcard please
er no. Anyway ... Git. I am, I mean I have to say
I was already impressed you know with Linux or Linux
oh I don't know how to pronounce his name! My Torvalds is really
knocking my socks off ... apparently it can also be called global information tracker
... it's just the interesting thing I think about Git, and we've got
... more about it I think in appendix five
of the ... of the book there so you know if you need some background reading
that's a great start ... but that
I think Linus was, Mr Torvalds
ah sorry I'm confused about pronouncing your name you doing this
huge ... you know this distributed development of Linux ...
of Linux, around the world you know developed
a version control system that met those needs and
... Git ended up; It's somewhat complicated ...
perhaps more than it needs to be in some places ... but
it's just so powerful, it's just so good for ... decentralized ...
teams and distributed teams you just - you just have to know about it really ...
also GitHub; we're great fans of GitHub ... that seems to be now it's like
it's almost difficult to talk about Git without talking about GitHub it's - it's
become
the most famous place to store Git repositories online
I think some people it's ... it's - Git by itself is ...
you know, Git is the protocol ... I guess for
ahh it's a protocol, it's also a piece of software ... for doing the version control and GitHub is then a cloud
hosting
service ... to host your Git repo - so
... the thing about about GitHub and indeed other ... I mean there are other ... BitBucket
and other people using
... git as well ... but basically if you're working as a -
as a team you need, as a distributed team, you need a central project repository
so you know GitHub is the largest code host on the planet; they're doing a fantastic job
they have ... their free tier is as long as it's all public ...
then everything's free and if you want to have private repositories ... I know for example
that with AgileVentures that's
absolutely fine. We do all of our ... you know all of our code is open source
and everything's done open development and we just you know I think there's a lot of
...
value to that, that ... transparency. Although there are other
you know if you go to BitBucket I think you can get free ... private repositories
for a small number and with GitHub you can pay them and get all of the great
GitHub stuff ... and a bit of privacy which I think is over-rated, but anyway
but that's another story the ... what GitHub has is the you know
they also got groups and so for example; actually we can go and see
if we go to Github and have a look at AgileVentures ooh, wo dee do dee do
Oh don't do that, oh, on no oh GitHub
yes go on AgileVentures yes
so AgileVentures and you know then we have teams and we have different sorts of teams
we can manage who has access to what and who can do - do what - it's all very
powerful and useful
... you know you've got integrated issue tracking ...
which I guess hmm, ... I don't know; we'll have a look maybe we'll see
... let's have a look - if we - we ... partly in AgileVentures
we don't use that issue so much because we're having such regular scrums
... every day that we're sort of talking about stuff face to face I guess if we go and
look at ... let's go and see LocalSupport but we got
... yeah the ...
there maybe the older version of this you know had
issues; but so you can see with these ... these issues as you know the people can you know
mention things that are issues with your projects and you know can sort of coordinate around
everything
really really really really useful ... you know that the pull requests which we'll
talk about more ... allows for this process of code overview
again super useful if you're on a centralised team but distributed teams,
wow! Just the ability for everybody to sort of look
carefully at what is being presented for integration into the main ...
codebase is really really useful - and and free wikis that everyone can edit and
that's just
really handy too - but so, before we wax too lyrical about GitHub
let's talk a bit more about about Git ... and you've probably done some things like
this
getting set up with your ... with Git at different points
... you know you can set up your default name and email I think if we go and have a look
down here I've probably got
let's got and see git config minus L I can list my config
oh I've thrown in a load of aliases but we can see my
username and email are ... are in there
already .... and so
it's as simple as you know you create a project folder and then you do
... git init and ... and then this then this there are certain things that
people get
tripped up on here I guess if we just sort of make a thing which would be
... let's call this git git test or something I don't know
and cd in there is - is this relationship between
the folder and the you know the git repository
because so to begin with if we're starting off here in git test there's
nothing in there
then I can do git init like this. The key thing to see
is that we've now got a dot git folder in there and we can do ...
for example ls -la dot git there
and we can see we've now got all this paraphernalia, all this infrastructure
directories set up to manage you know a git repository
and you can in principle you can just remove ...
that dot git directory and now ... the - the code that you have here is no longer
that's no longer a git repository. We can do it again: git init and its back and its
there it is. So generally you don't want to remove that, I mean unless ... and what sometimes is
and this is the kind of thing actually
... often people getting started with git run into the problem they may end up doing
git init
in a lower lower level directory and that can get
very confusing because really what you never want to see is you never want to
see ...
dot git in a lower-level directory and then also into a higher-level directory
... high-low so on and so forth ... I guess maybe there might be some justification for doing it
sometimes but that's ... that can often be - be a problem
but so here we are in this git test directory ; I've done git init
git init I've got nothing in there, let's maybe make ... what
could we have that we could have in there. We could have a README you know that would be a
good thing so we could do ...
touch ... README dot md is the sort of standard thing that we might have there
... let's have a look there; we have a README me now so if we do git status we can see
you know I have an untracked file and I can start
so this is the interesting, this is actually a two-stage process as many of you I am sure are
familiar
... with for how Git tracks and then
and creates a tr ... you know telling it first, you know if we do git add
dot would be all files. Let's do it for that particular one that README there, if we
do git add README now we've gone from a situation where
maybe I will make that window a little bit bigger we've gone from the situation that we had here
where README was untracked. We've now gone to the situation where it's being tracked
or it would potentially be tracked but it's - it's gone into this staging area
its not actually ... it's not actually been committed
into the repository and the - you know - until you do this
... git commit, for example like there we go git commit
minus m ... often it's the initial commit
like so; until we've done that we haven't we haven't got
... a, you know anything in our repository and sort of
so that ... two-stage process ... I guess it's - it's one;
you know make your changes .. two; add them to the repository and then commit them to the
repository
... is you know its powerful
because it allows you to do various subtle things with the you know,
not so much the order but you know you can make various sorts of changes
in different files and you can add them and so on so it's very very flexible and powerful but
but that's a lot because it's almost enough rope for you to hang yourself with
in that you can make ... you can think you fixed something by making changes and
then you want to push them to
... Heroku or to somewhere else and because you haven't
... added them or you haven't committed them or some issue and
you know ... I've been using Git you know all day every day for the last
I think its three years now and ... but still occasionally I will
have forgotten to do that but so particularly for people coming to
Git ... particularly if it's the first version repository system, ... version control
repository system that they've, or the first version control system that they've used that can be ...
very challenging and so good to be aware of you know
developers coming in to your team who are not necessarily so familiar with Git or version control ...
students ... other learners ...
but so ... if we want to make - what the -
we've got two create new projects - I think we got two slides
the same there ... let's move on ... but yeah - so this basic workflow that I've
I've - I've been referring to is that you've got your
you know directory that you're working in ... you can stage files, this is the add thing
to get them into the staging area and then you can ... commit them
and get them into the the repository ... and ...
you know that repository you know is then on your local machine you can in principle
check it out into other areas ... once you've got it up into the
the cloud on something like GitHub you know other - other developers can check that
out
and so on ... yeah we talked about the staging area ... this is this sort of flexibility
you know you can you can ... to be honest I tend to find I don't
use this power ... so much of the ability to sort of
... to commit
various things in stages I tend to want to go into a situation where
I basically have if we, if we look at the git status here that I have nothing to commit
here
and if I make a series of changes I'm gonna kind of be working on a
you know single user story, single feature, single chore just to get that stuff done
and then commit it in and and not do this clever mucking around with little bits and
pieces but ...
you know that ... power's there if you if you need it
... so yeah we we've looked at this ...
adding process that you know adding them different from actually committing
... I'm a, I'm a big fan of the doing this actually in one in one stage that for
example if we now
let ... README ... let's go in here and we say
... what have we got here this is ... this
you must read this, there you go, you must read this! there we
go and ... we exit out there. Now
... I would be very tempted to do git and even shorter to do git commit
minus a m ... you know updated README
like so and so that would, with the minus a flag,
add those things and actually collapse those two steps down to a to a
single step.
Thing to be aware of here is with this minus a, it will only work with the
the files that you already got being tracked, if you create a new file
so if we did ... touch ... let's have a look
... don't read me? I don't know I guess that's another one DONTREADME
dot MD ... if I now do ...
git commit minus a m updated, or created even
make sure your commit messages, hmmm DONTREADME
like so ... there's nothing - there's nothing added, it gives me a warning there, nothing added to commit but
untracked file present
so you you know if it's a new file that's not in the system then you do need to use
that git add. So there's another ...
there's always often these little places to ...
get caught out. Now to do this - this pushing thing
if you're just you know working individually on a single machine and you're just
you know you can carry on ... going through making changes
... you know ... adding things
rolling back the ... we'll have a video soon
associated with the Git Immersion assignment which will show a lot more
of - detail about that. Do do the ... Git Immersion tutorial is going to be part of this week's
assignments ... but more on all of the details on that
... later on ... kind of the
key things though is that like that's all very well just
on your local machine but ... the
you know Git has this - this set up to cope with
multiple ... reposit ... you can connect it to multiple repositories
so you've got this command "git push" which in its basic form will take two
arguments it will say git push
and then you'll have the name of a remote git repository
and the branch of that repository ... that you want to
you want to push to ... so we can have a look at
our remotes using this git remote minus v thing ...
and this is really ... at the moment we should see here that we haven't got
any any remotes there ... let's see if we're gonna go and
add ... something I could kinda go and get on GitHub and let's just go into my
... tansaku ... that's my
GitHub and let's go and create a new
repository and get in there and call this git
test ... and we'll just put test in there and make
that public and leave it like that there for the
moment ... you know so on GitHub creating your - your repository is as simple as that ... with that we now have a
remote repository in
in the cloud that has a a ... location. We can refer to it via
... HTTPS or SSH ... I find
I end up recommending everyone to use the HTTPS ... just because there's fewer
keys. There's
fewer setup but so it gives you these instructions here on how to create new
repository
and ... but you can push to an existing one which is what we've got here. So what I'm going to do is I'm now going to add
a remote there. We can do git ... remote add
like so "git remote add origin" ... now when I do git remote -v
we've got this is now the place ... we've sort of set that - this is
the origin - it's - it's - it doesn't have any special meaning but it's a kinda
convention that that says
that's going to be the main ... repository for this
you know the main cloud repository for this ... you know local developer
repository on our own machine and then by doing git push minus u
origin master what we will do is
we'll push our master branch which is by default is the first branch that we're on ...
and then ... we'll also set up with that minus u to say
you know we can say git push in the future and it would just assume origin of
master because that's usually want we want to do
... so now we're all set up with - with a remote. I kind of introduced
branches there which you may or may not be familiar with ... let's
go on and talk ... you can ... I guess you've got these
two different things to concern yourself with here. One is the the branches which are kind of
... you know you can create sort of alternate
parallel timelines for your code you can sort of split
at a certain point and say I've made these changes oh now I'm going to go back in time and I'm going to
split off
from another one ... you've also got these ... branches is one thing
... but then you've also got the different remotes in their different locations
and so ... one of the things that might
happen ... here let's ... all I've done here now let's have a look at our git test environment
there
so if I ... we now see that the ... the README
is there ... what ... one of the things - you can end up
and this is - this is - it'd be a common pass ... in some ways - sensibly - I maybe would have made this
in our organization like AgileVentures there
... but what I can do here is I can say I can ...
fork this ... actually this mirrors what we've ended up doing with ... Local
Support which started out
as you know my personal ... in my personal repository and we've moved it we've subsequently moved it
over
to AgileVentures this - this forking is completely different from branching; forking is
specific to GitHub
but so now by doing that simple fork operation we have a
a copy of the code ... ah not the code, this - this
repository on - on AgileVentures ... if we go back to the slides
we can see now but we might do ... you know get remote add upstream
so for example if I do git remote add upstream
this is now adding another remote
... in the list of remotes there ... you see even that the fetch and the push can be two different directions
if we go and look at that that's gonna have this URL. There's this
that is you can even get away but this they've got this special clone URL down here
with the dot git you can get away with
just using the one on the address bar it's sometimes a bit faster and easier to find
but so if we now add that as an upstream and I do "git remote -v" there
we can see we've got now in the list of other
... repositories that this git repository can talk to
are both this we've got the origin one here and we've got an upstream one
there and then you usually the way that it works
is the upstream one is gonna be ... the you know the group ... shared repository
and then the origin would be your kinda local developer repository
and so that gets you set up to ultimately to move towards pull requests and other similar
more complex things but so I can then in principle make
let's see if we go and a have a look, I can just do a - a
quick edit there ... edit here
what is it? "really you must" to the README
... online there usually you know you don't wanna be
doing it through the ... interface there but that's y'know handy sometimes and
in this case
so now that's gonna be automatically committed in the AgileVentures one
I can do things I think as we describe here in the slides where we say ...
"git upstream fetch" ... I don't have to do the ...
"git upstream fetch" ... "git fetch upstream"
so the - I guess the key relation there is - is - you know -
when you're pulling something it's doing fetch and then merge ... so if we do git fetch upstream
there
... that will the grab the upstream master
... and then having done that I can do git - you know - git merge
... upstream ... shall we do upstream/master like so
and then so that change there if we now do "more README.md" here then I've got
that change ... once we've I think done the first fetch
we could achieve ... the same thing, the fetch and the merge in one thing, by doing
"git pull upstream master" ... but
yes I mean ... there's this you know
the complexity of branching that ... is very very useful
... when you're developing different user stories
... and different you know working - working on things that it's not
critically required ... for the 169
Engineering Software as a Service course but you know really really really handy
and I think we go through the branching and checking out and sort of creating new branches
and so on in a fair amount of detail in the
the Git Immersion tutorial review that will come up in the homework section
... so you know I think more on that
there ... for the ... I guess what I will - I will say for this process
of ... branching and checking out and so on
fantastically useful for distributed teams doing things like GitHub pong and
... remote pair programming, which we'll talk more about next week and ... a little bit more
later on in these slides. Let's just talk a little bit more about what happens over at
GitHub. So you can see there how I sort of created some forks there
... the sort of model that we've certainly got AgileVentures and I think
repeated in many other places as well is that you have
a sort of organisation ... repository and then I mean if we go and look at
AgileVentures here we can see that sort of like WebSiteOne
is quite an active project we can see that's been forked twenty five times by different
people
this is all you know they'll all have that set as their upstream. We can go and have a
look here
at all the different people who have forked WebSiteOne
and so for example you know Thomas will have his own
branch and he'll have that checked out locally and he can then
you know just do you know everything he wants there try out different things
work on different bits of features
and so on and you know it's completely isolated from
anything that happens on AgileVentures WebSiteOne. So there's ... you know you basically get your
own playground
... which is - which is great fun ...
and then until you create a PR
pull request there and ... sometimes the interface for that can be
a little confusing I guess maybe we should just run through a quick pull
pull request there ... if we have a look ...
like so - so if I'm now in the situation where ...
all right, so do I still have the "DONTREADME" on there? If I do "git
add DONTREADME" on there
like so and then "git commit - m" 
... added "don't readme"
like so ... and then I do "git push origin master"
what I'm gonna do is I'm gonna get this change which is to add this file
... and push that on to my my local fork
fork in ... in the GitHub, so if we go tansaku git
test like so; is that the right one? ... we should see now we have a DONTREADME file
as well; doesn't have anything in it but there we go ... now I could do a pull request
... so we've got this green button here. I can say right,
and then you have to press "compare across forks" and so I'm going to look for, right
so this is I'm finding the top-level and I'm going to do a pull request from
... this is I always find the order of this ... its
its ... we're requesting that AgileVentures
... have I got this the wrong way round ...
it's correct I think ... so the change is one commit
"added don't readme" yeah, so that looks like the right commit, yes so we're ...
this but I always find that the "pull request", the term itself is kinda confusing
... for a
long time I was a bit confused about it, but it's basically we are
requesting ... here from our developer repository
we are requesting that AgileVentures, the AgileVentures, you know the big
you know upstream should pull in our change ... so I can sort of create a
pull request, we should always you know ... explain what we're doing
... you know to help our project manager know what we're contributing
we do send pull requests - and then - so now actually because ...
you know I have admin status on AgileVentures it's taken me directly to AgileVentures
here
and we can look through and see what files were changed. There are no ...
and we can see there is a commit and so on and then
so you know imagine that you know a different developer has submitted that
from the team I can now, you know, review the code. Other people can all now look through it. This
becomes
if we look now ... AgileVentures git test here
anybody can view the different pull requests that are coming through ...
and maybe we go see some examples
... probably got some outstanding pull requests there, yeah,
so this is you know ... we've got John there has got a pull request. I can see the
changes that he's made.
This is just absolutely huge I mean both for centralised teams, but for distributed teams
you know everybody ... the visibility of the code that everybody's submitting, it's
absolutely huge. If we just get back to ...
our little git test environment there
we can see that we've got a pull request and then as the project manager I might come in and
have a look through and say
you know I might make comments and say things. Ultimately I would say alright oh yes let's
merge that pull request hopefully
and ... that gets merged in and so now when we go to AgileVentures
... git test like so we've got that change is incorporated in there. So this
its fantastically powerful this if you"re doing it in open source
free framework in order to pull in ...
contributions from developers potentially all around the world and ...
you know everybody - you know - people have been doing this - you know -
much longer than I've - I've been thinking about it but it is - is fantastically powerful
and you know not particularly required -
for the 169 Engineering Software as a Service course but
y'know it's kind of once you've got the Git skills and Heroku skills and so on you're -
you're
set up really to do things as we've been doing them at AgileVentures which is to
have
you know your organization and your different projects and have people
contribute
to them ... you know from anywhere in the world and you know
be getting together whether it's you're doing it entirely asynchronously or doing it synchronously
like we do which is
getting together in team scrums to discuss the features and the pull requests
... it is extraordinarily powerful so ...
yeah I guess just to touch on you know we can also use
you know GitHub ... Git using push and pull you can GitHub pong which we'll talk
more about next week
and which I'm a big fan, though there are many different mechanisms to support
... remote pair programming which I mean pair programming is just my thing
and I think remote pair programming incredibly convenient and my favourite is GitHub Pong, but
more about that
next week and there's there's a lot more. Git is an extraordinary power tool
and ... you know we can hardly do it justice here there is a lot more reading;
I mentioned already appendix 5 ... of the textbook that's definitely,
do check that out ... there's a great
this is a great ... what do you ... It's a PDF document by John
Wiegley
about Git from the Bottom Up which goes through .. it's not it's not that long
I really really ... we ask you to read this before
attempting the Git Immersion ... homework
this this this week ... more of that later
there's also this entire book on Git. I personally haven't found myself
with the free time to go to read all of this I tend to dip in and out of it ...
but that is a fantastic resource. And I think we've also got another thing which you should definitely check out 
is this visual guide to version control in general so lots of fantastic resources out
there
but I would say you know extensive use is the big teacher that's partly why I'm such a
fan
of GitHub Pong is because it basically forces you to insert
continual ... git interactions into your
programming and pairing process and you know that there's nothing like
continually using git in order to finally you know
get ... the context of it. We haven't touched on branches ...
there there there are some kind of issues like ... the way that
branches are managed. I ... took me a long time moving from
other version control systems to kind of really fully understand
those ... we'll talk more about it in the Git Immersion
tutorial support. But there we go - that's it for version control for the moment.
