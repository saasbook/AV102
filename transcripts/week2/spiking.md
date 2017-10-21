<a href=https://edge.edx.org/assets/courseware/v1/b934f339b12e2d3ba8d93f712702a5e4/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/2.6-_The_Concept_of_Spiking.pdf>Lecture Slides</a>

Hey so I want to talk to you about spiking or
doing a spike; which is an important part I think particularly of working with - well
any team. Like so many of these different ... software development practices
... they can be very important - both in the distributed team and
you know - in a centralised team, shall we say - working in a single - single office
I want to give you as many examples as I can, for how
spiking you know can be used in distributed teams.
So spiking, or a spike is a special type
of Agile ... story or chore you can kinda see it ...
as a bit of either. It doesn't usually have any points associated with it so
perhaps more on the side of a chore ... and
the key thing that the spike is for is to try and drive out risk and
uncertainty
... it may be that, you know, some of the situations where you're trying to vote
on stories in your team; members coming together and saying well, you know, that how
trying to work out how hard something's gonna be to do - that you just don't have
the technical background; it's a new technology, it's a new library
what have you ... so you need to do some sort of technical investigation
and just kinda get something working ... perhaps without tests - this is one of the
... areas where you can still of put down the BDD/
TDD mantra and say right you know okay
we're gonna to just sort of investigate doing some code; see if we can get something working
to give us the information to estimate how long it will take to properly
BDD a particular - particular - story and so
the idea is that this would fit in a single sprint with a few iterations sizes of
you know
a week or two weeks or five weeks of whatever it happens to be. What you really don't want to be
... is in a situation where you are - you do sort of a spike
it's like oh yes, this is working and then you sort of end up working on it for weeks and weeks and you
ship it and then your
you know ... the customers is like is using and depends on that.
I mean this is basically kinda the ... the bad old days was one long
spike.
There were no tests ... it just you know sort of made it work
and occasionally there were bugs in it, like right because we've just got to keep bashing at it until we can fix it
...
but so you know that behaviour if you've ever
gone on that is called spiking and it has a special role
in the whole Agile process; that as I've been talking about
the motivation is really to familiarise ... your team
... some of the individuals with a new technology domain you know
... you want to kind of work out ...
you know what the behaviour is going to be so that ... you know ultimately you can
estimate
the story effectively. I mean any estimation process is always gonna be
riven by uncertainties but sometimes if you just don't have the information
you're estimate is going to be really poor. So we can sort of
split these things into you know sometimes it's going to be more a
technical spike where you're just okay this is this
... library that may be automates some portion of
the system that we're you know currently delivering and
and you want to you know get that get that sorted out
... or it might be more of a functional one where
... you're trying to understand the user interaction and sometimes
it's gonna be a combination - a combination of the two ... I've got a couple of
slides here on,
first on technical spikes - yeah you know you're -
you know you might have ... multiple libraries that - 
you know - you would be using in order to
solve some sort of problem so you might wanna do a spike where you
try each of those libraries in turn ... to evaluate the performance
... see how they work under load and so on and you know you wouldn't
necessarily have to drive
all of that through tests. Although you know you still could use tests as
part of a spike.
Yeah and really you know you just wanna understand
as much as you can about the particular approach before you can't commit
to any functionality and we've done technical spikes
on for example the AgileVentures EduChat projects where
different people involved in that would evaluate you know ...
an XMPP solution or an IRC solution ... and kind of go away ...
this is a distributed team. I guess again, it doesn't really matter
from the ... general perspective
whether your team is you know spread out over the world
or whether they're sitting in the office given that you've got multiple people on your team
you can, you know, split up - you know - looking at different technologies
across those team members.
Yeah so I think this is one of those things that ...
you know - it's not peculiar at all to ...
distributed software development but it is fantastically useful
and it's the kind of thing that's you know if you get involved
in development involves the Agile process or you know
large numbers of people understanding this terminology you know very very
important. We find it
to be particularly useful in our discussions as part of Agile Ventures.
We can also refer to to a functional spike
where you're unsure about how the users going to interact with the system.
We also sort of refer to this as maybe as LoFi prototyping.
You kinda wanna get user input on what a
you know how they would interact with the system before ...
before you've actually had to build it and this is often delivered
as a user interface mockup ... wireframes
page flows and so on. There's also Wizard of OZing.
You can sort of pretend you're computer putting up pieces of paper
and having you know a user click, as it were, click
on them at different locations to simulate them interacting
with the interface ... we've actually we've just
at this very moment in AgileVentures and in the LocalSupport
project ... we're working on ... we've had a spike
being developed by one developer ... just for reference
this is the existing ... sites for LocalSupport
it's a directory of nonprofit organisations
in North West London. We've got this embedded map
in there. The details of the project not so important in this example but one of the things we've been talking about
with the client
is breaking the map out of this box and making it kind of
go full width screen in much the same way as recently Google Maps
has done and so one developer has
spiked that. They've done here a mock-up of
what this would look like and we showed this to the
client
today and the client was pleased and was able to play around
with this. Here we're not using - you know - we were not using (mockups)
we've actually built the thing partly because
Google Maps had already - you know - in this case
we didn't really need to have a mock-up
done on paper and so on because Google maps had already blazed a
trail
there to show what it would look like in there and the client already knew that they
were interested in something like that and so
you know rather than trying to just create stories about
and vote on that since we haven't done a full width map before
it made sense to spike something just see if we could get it working
particularly as it involves interface elements, CSS and all this
different stuff
... it makes a lot of sense to see if you can just get it to work and
it does approximately work. There's you know not every piece of functionality in the site
works but we've demonstrated that it's possible in principle
and this one is the functionality of getting it all to display
correctly getting certain things like we've got sort of pop ups appearing
and this that and the other; make sure that that all works
and also that the clients is happy with that.
Sort of the key thing we go back to the slides there you know
having created the spike like that it's not that
now gets shipped. It's all about can we use that as a
... estimation framework ... and so what we've done now if we go to the
Pivotal
Tracker for LocalSupport there is we've now got a full width map epic
and we've begun the process of breaking out all the different components
that make up this whole map transition
into individual stories that we'll then be considering
independently in voting on them and then driving with tests as a way to ultimately
deliver
this full width map view to the customer.
So really the spike it's gotta be providing you
information that helps you estimate the stories that are ultimately going to go in there.
It's gotta have ... it's gotta actually
work ... that's the key thing. I mean what you may find of course in a spike
is you demonstrates that it's just not gonna work or it's going to be extraordinarily
hard
to get what you want from a particular piece of technology, so that's very
important and it needs to be something that
can be ... particularly it makes sense in the user interface thing
you know that the client can accept or reject based upon
you know what they're seeing is going on ...
if there's not a user front end then you've got things like
performance and so on but you've got to have something measurable that
can be, you know, accepted right - that this response time is acceptable or not -
... the key thing really is that the spike should be an exception
and not the rule. Every story there's always going to be some level
of uncertainty; but you really don't wanna spend all of your time spiking
and you know adding tests as an afterthought. Really
the spike, I mean in the
classic approach that you would do the spike and you would then throw away
that code
and you would then re-drive development via
tests using the knowledge that you had learned by doing the spike
... yes ... so this is - you need to
accept a certain level of uncertainty that's what the ...
the process of voting on stories is all about - and yes spiking
should be your ... it's one additional thing in your toolbox which should be
reserved for - you know - where you really, particularly as a team
don't know ... what's going on ... so in conclusion
you know - spiking is a good method to gain a better understanding of the
stories and
to lower uncertainties and - you know - that side of things
needs to be organised as a team. So that - you know - you're sort of
working out as a group. That you're talking about developing a particular kind of
feature and asking about "Have any of you tried this before?"
and you know again, whether you are in a centralised location
... or you're distributed around the world; I mean the key thing is communication
and so you need to be having ... regular scrums or standups or
what have you in order to be talking to the team members and saying you know
we're thinking about this feature for the client ...
you know has anybody had any experience with anything about using
this library, this piece of technology?
... that communication process is absolutely critical
and the key difference really for distributed teams versus centralised teams
is making sure that that communication flows whether it's
whether it's with ... you know instant messaging or ...
the emails or you know the face to face hangouts and so on
you know all critical communication technologies that we'll be talking about
more next week
