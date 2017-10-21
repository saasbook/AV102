https://edge.edx.org/assets/courseware/v1/9442a740c7eb674f2fab347a359e389d/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/3.5-_Github_Pong.pdf

So let's talk about GitHub pong. It's my favourite kind of
remote paring strategy. There're actually, there are lots of fantastic tools
for remote pairing such as, what was it, ScreenHero
... Cloud9, Nitrous ... Floobits. There's just ... there's lots and lots of
them
... but one of the things - like this GitHub pong procedure
I really like: One because it leaves a trace
in the GitHub commits that shows ... how people have actually done the
ponging ... and also it just you know it constantly polishes your Git skills
and your understanding of branches
and so on ... and it's pretty fast and
I love it personally ... but so basically what it is ... I mean you can
with GitHub you could give ... everybody
access to your repository and they can they can push and pull.
The nice thing about GitHub pong is you can ...
have a situation where someone's ... you're working on a repository; someone else forks that repository
and so they've got a copy of the code but then you can ...
there's this sort of crossover thing which eventually we'll have a good diagram for;
but where you ... can both push to your own repositories, pull from each
other's repositories
and do this kind of GitHub pong. I've got a video of us
doing its ... which will follow this up; but ... yeah
its ... I love it for
remote pairing and combine this with
some sort of screen share; whatever you fancy: Google Hangouts, Skype
doesn't matter, WebEX ... any screen share system
plus GitHub pong, you've got I think a good remote pairing
solution ... for screen share I'm assuming you've got
reasonable bandwidth there. So ... the way to do it is that you'll
fork and clone
... the GitHub repo that you want to work on
... then you go through and add your partner as a remote
... so here this partner name that can be
... their first time or whatever ... and then
the URL to their remote GitHub repository ...
just check that it's in there properly and then
you can fetch a working branch from the latest code ... usually
depending on how it goes ... you might ... I guess that you'd often call
if that was the ... you'll often have forked ...
like an AgileVentures ...
open source project that would then be ... you'd often call that the
upstream ... it maybe that ...
if you're just working ... if there's sort of like
two of you both working on a - on an existing codebase you - you might have
forked each other; so whether you call this upstream or you gave it your partner's name
... may vary slightly but so ...
you can then check out a copy at that and this is getting setup and then
... do "checkout -b" to create a branch based on that
and I think actually if you're
... say for example that I was working with Jon, I'd do "git fetch jon"
I might check out Jon; this would be like his feature branch
... like so and then I would do checkout
minus B feature-branch and then I would have a
precise copy of Jon's
feature locally ... I could then
start off driving; I could do some work; I could
do our commit message and then ...
I would do like so, I would do one side done,
my part so let's say "make it work" ... we've got a feature branch there
I would say "right I've done my bit" maybe
I've written a test the code that we wish we had; verified the test fails and
I would
commit and push that up to feature branch and now
for the second half of the pong, what the partner B would do, they would
... and probably the first time around they might do this "git fetch a"
but in future once they're all set up
then you can just do "git pull
feature branch" there and at A insert the name of your
partner
and you then get an exact copy of their code
and ideally you immediately - you run the test just to double-check that
there isn't anything
hanging around but then you write the simplest code that will make the test pass;
refactor the code; next failing test; commit some pushes
and round and around and around
... and if that didn't make so much sense we've got a nice video coming
up
of that in action and I think you'll agree
it's pretty pongy. Alright.
