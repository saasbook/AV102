https://edge.edx.org/assets/courseware/v1/4fd041e85ec6cd61ab16d24bc10f7e39/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/3.6-_Github_For_Teams.pdf

Well let's talk about GitHub for teams and I've got
my friend Paul here with me and in a second we're going to have a
look at some pull requests ... I always found
the term "pull request" to be somewhat confusing
... it sort of like which direction is it? sorry?
kind of going in? If we go to GitHub and we look for example at
oh I don't know, AgileVentures autograder examples
and I think we've got some pull requests
in there but just so the idea of like, who is it? where is it?
I guess now in my mind I got it relatively straight of okay so I'm
sort of project manager on the autograder stuff, I created this
repository
on the AgileVentures site and that's up there.
Now, anybody else in the world can say "Right I've made a change to some code ... they've
forked it, we can see a list of the people who've forked this repository
over here ... and the network graph always seems
to take a while but anyway all these people have forked the
AutograderExamples; they've got an entire clone as it were. Well clone is an unfortunate term because of course you
use that to 'git clone', to 'git pull' stuff on to your local machine but
by having a fork
all of these other users have their own copy of 
AutograderExamples ... both in the cloud on GitHub and potentially on their own
machine. If we go back and look at ...
the pull request then, a pull request is
somebody saying: "look I've made some changes and I would like you to pull them in
to your code base" ... and
Paul's becoming an expert on pull requests. We'll just
... and I'm becoming more and more of an expert on merging them ...
so the process of preparing a pull request is basically that ...
you have ... you push your stuff that you want to a
feature branch
on your fork and then when you get through
to GitHub you need to switch to that branch and you'll find this
pull requests button. It's sometimes a
little bit difficult to find. I find the process of
getting the pull request to point to the right location is sometimes
... a little bit challenging ...
I wonder if ... have we got a ...
let me just think, if I grab a terminal window
... like so and get into the
... get into AgileVentures here
AgileVentures and the AutograderExamples
let's pull an old terminal window in over here
... so I think we've actually maybe
only got a master ... this is a relatively new project, we've only got the ...
oh yes we've now got a develop branch ... so
"git checkout develop" and
let's have a look. We've got there ... we've got the README. So I could do a very quick
change to the README there ... for example
I could just add ... a
let's put it in right here. Testing pull request
like so. So I've made there some change
and then if I do my "git status" here on the ...
I've got a modified README so I could do git commit minus A M
... there and say testing pull request
like so and then do "git push
origin develop"; in this case I'm just ... partly it's
... oh yeah, ... oh you don't want ... oh dear I'll have to fix that and you will have to make sure
that ... you've got the latest code
as well otherwise you get these fast forward things and we'll do
merge there ... let's try again "git push
origin develop" and so
one of the nice things actually GitHub will provide, often provides now; if I now go to GitHub
and I reload
this page it'll actually ... or usually ... I guess ...
if you're doing ... that's funny, let's go over to develop and have a look. Recently in GitHub
I believe it often has a pointer of what ... here's a recent commit ...
has that actually pushed up properly? Let's go and have a look, yeah "git push origin develop"
AutoGrader AgileVentures yeah - We're in the right place? - yes - so we've gone to develop here
... yeah, sometimes I get a little
thing that pops up here saying "Oh you've done a
submission recently would you like to be
pushing that here there and everywhere"; I think that's maybe only when you're on a fork
but I can come in here to a pull request here
I've pushed that up into develop there it ... you've got this green button "new pull request"
and then you get this process where ooh yes you can compare across forks
and so in this case I might just say I want ... and I always find this confusing
it's like ... I want to get the develop
and then the base here is the master so here I could create a pull
request
and this would be me saying "Right this change that I've made to the README file
I want to have that go into the
the master branch" ... but potentially if I was on somewhere else, I might say
I want to compare across forks and I could do a pull request over to Paul's
thing here so for example; so base fork, aah it's confused there ... so if we take that's Paul's
repo and I could for example here this would be me saying right
I want this change - this recent changeset that I've done to AgileVentures'
develop
I want to push that over to Paul's master branch
and I might say okay rather than his master I might wanna send this to
his develop and so this would be me
sending now from our kind of upstream pull request back down to Paul's develop;
which'd be a little bit strange but at least you're seeing the interface
here there's this ... you click this button to create the pull request
and then you describe what you're doing and you make sure you
leave
sensible comments so the person who would later on merge your pull request
knows what's going on so ... I think that's the key thing
there, I mean you can review the changes - actually I guess - did I
didn't ... we can see there a list of the changes there
... personally as a person who is often merging lots of pull requests
I say the simpler the set of files that's coming up; the smaller the number of files, the smaller the number of
changes
the better ... that's all ... makes it much more easy to manage
... but yeah make sure that you describe the pull request
and then you're done and you'll end up
in a situation where the administrator of the project that you're
pushing to ... if we now ... can I now
yeah, maybe there ... we'll have a situation like this so here we've got
previous pull requests that Paul has submitted to me
... let's go and have a look over here [Paul] oh did you not submit that one?
[Sam] I think I didn't submit that one; that would have been just a spurious one to submit [Paul] gotcha
[Sam] to you I was just sort of ... I kinda; we
... I think that the ... I find the interface for kinda going through that
a little bit counter-intuitive; we've mentioned
some of the things there.
At least knowing where to find the button is kind of a key thing
setting up to do a pull request [Paul] a lot of the ... every time you select
the branch it will jump back to
where you have to click to edit button [Sam] yes yes
there's definitely ... I love pull requests; there's definitely
a couple of HCI issues there in
the GitHub interface, but yeah and so actually as part of
the whole 169 course you are never required to make a pull
request but they are if you're working with a distributed team
... such as for the autograders, they are the lifeblood
are they not Paul? Its being able to do ... [Paul] it's how things get done!
[Sam] yeah absolutely that's how people
contribute into the center; so to a certain extent
in the first instance if you're just ... you might be getting used to
submitting
pull requests ... then there's the process of you actually being - sort of managing an open
source project or managing
a private project for that matter, but then want to merge these pull requests
and so what you'll get is a status. git will check if it can merge automatically
... so for example if we look here ...
we've got this thing for helping with continuous integration
work on the autograders and we've got Travis installed and so that tells us
that all of the tests have passed and that's great to have
we are hoping this time around in the in the 169 MOOC to include a continuous
integration
homework we'll see about that, maybe we can even work a pull request
thing in there, that would be good I think but so I can now ...
assuming that I'm happy with this and I often ... I'll be
here as me as the person who might be doing the merging. I'm like right
yes ... we're setting up so we can use our
GitHub API keys to
do certain sorts of testing in the autograder; good show,
and the files changed I can look through. We've got
some features changed there, we've got some
steps that support them ... using Travis
secure key and so on ... I've looked through this
in the past and think I've identified that I'm pretty happy with it ... and it's always
fantastic to see ...
... this is a lovely size ... three files changed
one of them is a Cucumber feature, another one is a
spec and then there we go and maybe a little bit of application code
actually this project is a lot about updating the continuous integration
so this is the kind of thing, the kind of size
of pull request that as a person looking to kind of get merged
developers' code in as quickly as possible I love to see
so I think we can we can have ... I mean we're also being told here 1) that there's no
conflicts
and 2) that all the tests have passed so I'm very happy to merge that pull request.
It does give you a second chance, but having done so
we end up in this situation here and we go back and this code is now
pulled into ... so that was from Paul's develop branch into the main
AgileVentures'
develop branch there. We now see that pull request
has gone from the open to the closed side
and I can now get that code on my local machine here
I can do "git pull origin develop"
like so and then I've got
my copy of that code and I can do things like
deploy it to production and so on and so forth
... so that the process of merging
pull requests ... the other thing that you can ... you may find yourself doing as
a project manager
is doing cherry-picking where somebody may have submitted a pull request
and in this case let's go back to the one that Paul had
there. It was this one wasn't it ... so the actual - we can look at the commits.
There was - three commits - and it was sort of a coherent whole
there was no
need to - to break it up ... probably the best example I think that I
had of a pull request ... if we just go to a different project this
was earlier on on LocalSupport ...
I guess rather than going to another Autograders one and doing
... let's go and see here. If we go into LocalSupport
there was some people who got involved and did
some pull requests on LocalSupport and
... they were relatively like ... I wonder if we can go, if we can quickly find
they're gonna be sufficiently long ago
that I can't find them, let's see
dn da dn da dah. That was by Daniel and not the surname
but ... mmm
yeah there's so many pull requests from ...
yeah that was from before Christmas mmmm anyway let's let's since I can't immediately
find that, let's take ... another pull
request from the AutoGraderExamples and go in and so we might see
which was is, let's see which one is more complex
... again not so complex but say for example
thats on reviewing this pull request I decided well yes actually I want
these three commits but I don't want this last one
... assuming I've got an ongoing dialogue with someone like Paul which
at the moment I have which is fantastic ... I might be able to say "please update your pull request; maybe
you could remove
that commit" or what have you ... I might be wanting
just to pull in ... certain elements; certain of
these commits and if ... that would involve me
doing cherry-picking and so basically I would
check out a
version of Paul's code locally ... so for example if we look at
if we look at this, Paul's got that on a tags
branch there so I might for example I might do "git
fetch Paul" here I've already ... I'll show you, I'm set up with
Paul as a remote. I'm going to do "git fetch
Paul" like so ... and I'll then see I've got his tags thing
so I could then do ...
"git checkout paul tags" and is very similar to the startup for
GitHub pong ... but rather than create my own
tags branch as I would be doing if we were going to start doing a bit of GitHub pong,
now I've got access to his ... I
... actually I didn't need to checkout I could have just fetched it
but so I could be exploring things in this. Particularly before even
deciding to do
a cherry picking or a merge, this is very very handy to be able to check out that
person's
entire code as it was and sort of play with it
in the environment on my own computer; that's extraordinarily useful ...
but so what I might for example be able to do if I might just go "git checkout develop"
what I could be doing here
is I could be grabbing ... just saying that I want to merge ... I could be doing something
like
git cherry-pick and then
... yep cherry-pick
go on ... yep and then ... there we go
so that would be that would be me grabbing just
this ... let's say
just this commit out of these four or whatever I fancied
and then playing with it until I got it to work on so and so forth. So
... and then you know if Paul himself wasn't available to update the
pull request
then I might well just end up cherry-picking a few things
and then closing it and maybe opening a new pull request if
I'm not the project manager but there we go so
... I would say ...
distributed teams this sort of ... for the process of making pull requests,
merging pull requests,
cherry-picking, triaging them handling them ... that's the life
blood
of what we do in AgileVentures and the best way to get experience with it is to keep
to just do it! I mean there are many many other open source projects besides
AgileVentures but we will be very happy to help you
plan and experience all of these things in regular Hangouts,
one-to-one, face-to-face so to speak; if you can call Google Hangouts face-to-face
Alright ... I think we'll have to say goodbye for this week and look forward to seeing you
next week
