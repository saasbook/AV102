<a href=https://edge.edx.org/assets/courseware/v1/bc58799de258a9c219207dde169cb9b2/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/2.3-_BDD-TDD.pdf>Lecture Slides</a>

Hey, so I want to talk to you about the BDD TDD cycle  versus, or is it the same as the acceptance/unit test cycle.

Two key concepts that are related in strange curious ways  let's talk first about BDD and TDD.

Now as you probably know BDD stands for Behaviour  Driven Development and TDD stands the Test Driven Development.
<a href=https://edge.edx.org/assets/courseware/v1/bc58799de258a9c219207dde169cb9b2/asset-v1:AgileVentures+AV102+Spring_2017+type@asset+block/2.3-_BDD-TDD.pdf>Lecture Slides</a>

Hey, so I want to talk to you about the BDD TDD cycle  versus, or is it the same as the acceptance/unit test cycle.

Two key concepts that are related in strange curious ways  let's talk first about BDD and TDD.

Now as you probably know BDD stands for Behaviour  Driven Development and TDD stands the Test Driven Development.

I think there's often confusion about what these are and the difference between them
I see them - I personally see them - as pretty much the same thing
... I would argue that maybe TDD is the bigger set
... and you know BDD is kinda a subset
of TDD ... the key thing you know and ... I'm not the
Oracle on this but seems to me that in order for something to be behaviour driven development
you need to have a higher-level description of the expected behaviour
you need to have something that's that's ... comprehensible
to someone who doesn't know your code ... inside and out
... and so I mean I think the term Behaviour Driven Development was developed by the
people who
developed RSpec and Cucumber ... I think although that JBehave was the
original
precursor and I think the idea was to move away from the
... the test, ... I mean it's still you know Behaviour Driven Development still has this same sort of
flow
in that you know describe a behavior that you don't yet have
implement that behaviour ... you know ... see that - you know -
... that that's ... there's that in place
with the, ... it sorta, ... to test - Test Driven Development
is that same flow but the Behaviour Driven Development y'know, it says, right -
we can't just specify low-level tests we have to
specify the high-level behavior and so some tools in fact both
RSpec and Cucumber ... by their creators are suggested to be
BDD tools because they can describe things
at that, ... sort of a higher-level
now there's maybe some confusion that arises from this in the course
in that the 169 Engineering Software as a Service course
because we we ... breakup certain homeworks as we talk about the BDD
TDD cycle ... we have a homework which involves writing cucumber stories which
is
labelled a BDD homework we have ... the following
homework which is called BDD/TDD cycle which involves doing
both Cucumber and RSpec and I think one can come away with the impression that
somehow
"right ... oh yes cucumber is BDD RSpec is TDD"
that's what that's what happens ... and there are diagrams
that support this the you know and
you know I think the ... this concept is is around
so frequently that we can't kind of ignore it ... I feel
that it maybe ... I dunno it's not the most accurate way of
representing this. Whatever we call it, this process of having
... am higher-level feature tests and lower-level, shall we call them, unit tests
... and sort of swapping from one to the other and going backwards and forwards
is extraordinarily powerful ...
in in some ways I don't get too wrapped up in the debate about what the
terminology, y'know how we describe it ... I think this
process with your centralized team of a distributed team
... you know even in your individual you know just this process of working
fundamentally can massively improve the quality of the software
that you that you generate. It's - it's not a - a magical elixir, but its - it really
really really can be a huge help and
you know we we're seeing that all the time in the y'know distributed teams
working on AgileVentures but just to go through you know as it's described in the
terms of BDD/TDD
the idea is that you would start by having a failing feature test
... there we've got the red arrows representing that so you got we've described sort of the high
level feature, the high-level behaviour that we want our software to have,
it doesn't have it. We would then rather then immediately making
that ... pass we would drop down to a low level and we would write
a lower-level test ... that would also also be you know it was described here as
writing a failing test, a unit test
we see that fail. So then we're in this thing we have like two levels of red
above us; we've got a failing feature test
and then a failing unit test and then we will actually implement the code that we wish
we
we had and make that lower-level test pass.
We would then refactor as we've ... heard talked about in the main course many
times
... and then ... ideally what will happen
is that as a consequence the ... high-level features test, because we've,
of course, done all our unit tests correctly, the high-level feature test ...
will will also pass ... of course there may be
you know it may be that ... for the high-level feature relying upon
several you know different individual unit tests that they might be
several several cycles there but ... and
well ... One: this is like I would say one the most powerful concepts
from from the course and in software engineering and I'm a big fan
... however I do worry about people calling it BDD/TDD cycle
... I prefer to call it acceptance test
unit test, or acceptance/unit test cycle let's talk about what we mean by acceptance
integration and unit tests
... particularly when I talk about these tests acceptance tests
coming from sort of an extreme programming background I'm talking about
just checking the entire stack, checking that there's the function you know all
of the functionality its present
I think depending upon where you're coming from that might be called system testing
and acceptance testing is when you actually put something in front of the
customer
... you know that ... I think again all of these terms
they're they're though the actual words; they're guides
like I think to get too hung up on what exactly
these things mean is to is to miss the wood for the trees ...
you know Wikipedia has a good article on all the different types of software testing
you know that's a - that's a - that's a great read ... but I I think
here what I want to do is try and ... focus on this -
this process and not get confused about ... you know
which tools go - go in where. Anyway listen - that's acceptance tests
which are kind of the higher-level tests and they are checking that things are really working
almost like from the perspective of the customer
.... then you ... sort of at a lower-level down you have integration tests
that will be checking that ... a couple of different components in your system
are working well together and then unit tests being y'know single unit; that's checking
a single component
of your system and that give's us a diagram like this; there are many diagrams
out there ... I don't know that any of them are yet perfect we're still in search of ...
perhaps we will one day draw the perfect diagram, but
... you know I think rather than the
BDD/TDD, I think calling the top level
cycle of red/green/refactor the acceptance test cycle and the
smaller lower-level ... things the unit test cycles
they is is is better because the problem is that some people
... use RSpec to write their ... high-level feature tests
and ... you know although in the
... Engineering Software as a Service course we've used cucumber
for ... the behaviour ... sorry for the feature tests. I'm getting confused myself!
we've used ... cucumber for the high level and ...
RSpec for the for the lower-level ... you don't have to do it that way round
I mean that you can argue that they lend themselves to those different levels
but it's not it's not required and so
... I think all this BDD/TDD is missing
the key point which is that you're you're ... whether you're using
... Cucumber or RSpec or even you're writing your own hand rolled framework
the key thing is that you have a high-level focus the you're
somehow attached to some ... user story or business value
right. And that there's some of ... you've got some sort of failing test
that represents that. Whether you're calling that you know
your feature test or you're calling it your acceptance test ... doesn't really matter
but the key thing is that you have that
and that that's your high level focus and
that you're then you know not relying solely on that but you're also
... testing the little components and the interfaces between them because your
high level tests will tend to run
rather slow and you can get ... you know
... it will tend to run rather slow and it may rely upon a whole cascade
of things and it's difficult to write tests for all of the different possible ways ...
the pathways through that. That's where your smaller y'know unit tests they allow
you to to focus on on a low level thing
but whenever you're working on a on your test you should be able to say what your
high level acceptance test is and often
people are asking me for help online; they're saying I've got this little tiny problem
here and it's stuck or it's not doing this thing
and I - the first thing I say is - the first thing I think is, actually, what I say is
you know ... what's the ... what's the chore or story that you're working on in the
bigger picture of the project, 'cause I want to understand that
and then I say right okay what's the acceptance test issue and then what's the unit test
issue
and the final we'll ... finally we'll look at whatever comes up
in the actual application code ... so this this is a pretty good diagram I
think
... it doesn't really show the flow from you know okay you've got an acceptance test cycle and its
you've got unit test cycles
embedded within it. It doesn't show about the
flow in quite the way that I wanted. This is another good - good
... diagram ... although because the arrows are not numbered
I think it can be ... somewhat confusing I think the way that its supposed to be
read is that you so start here
and ... on the top level here we've what you know top
circle or the outer circle with the acceptance test and you would initially have
a an acceptance test going red which might be in Cucumber, might be in RSpec but anyway
... you have that going red and then you would drop ... the first thing you do is you
drop down here. Now
failing acceptance test means it's now time to ...
have a failing unit test which you then make it pass and then you refactor
and then once you've got you know some number of unit tests
... passing sufficiently so who you think you've got all the ones that are part of this high-level
feature
you would then jump back out and hopefully see your high level acceptance test
pass and then you might do some refactoring there so this is this is a pretty
good diagram
I like this one I just yeah it needs numbers and an explanation to go with it
but this I believe is based upon what I would almost call the missing manual
y'know I think this
RSpec book ... which is all about RSpec and Cucumber
and friends is just excellent I couldn't I can't recommend it enough
... I think it's an excellent ... addition to the
Engineering Software as a Service textbook ... a lot of the material
from the RSpec book is in I think it's all there if you look it's it's all there
the ... this is I think such an important topic
that you know ... the way that it is presented
independently of Rails and you know Software as a Service and so on
... it's it's it's it's really really handy ...
but so that ... previous diagram - that comes from a diagram
from the the RSpec
... RSpec book which ... is the same, it doesn't have the colours but it does have the numbers so you can see
... this process here. It's a little bit of ... and it is the same thing
again but it's also got that if we look at it in
in text there ... so the and
... in the RSpec book as in the ... the ESaaS
course it ... the suggestion is to start to use cucumber as your higher-level testing
tool
... that's for features for acceptance tests and you know you you
focus on one scenario
you write a failing step definition. You drop down to,
you know, having done that you then drop down to RSpec you
write a failing example to get the example to pass. You refactor
and then you know go around around around and there's lots of excellent
... examples in the in the RSpec
book and you know I think the the challenge in some ways that we have with
the bigger ESaaS course with the
Rails and everything else that is being presented; it's
almost not until part 2 of the course that you actually get to practice
... this - this process ... and I was wondering I think I might just do
a little sort of concrete example of that on the command line; we'll see if and if this a
blows up in my face but if we wanna have ... just a simple
let's see. First I wanna do, so this is going to be I'm going to call this
`acceptance_unit` 'cause I wanna move away from BDD/TDD
let's go inside there and what I could possibly do is I could do
a features directory which we would ... need for cucumber
and then I could do something like ... nano
features ... now and I'm going to sort of adapt
... an example from the beginning of the RSpec
book here we'll call this ...
let's call this the greeter feature
... like so, there we go
and so we'll have a feature here that says
Greeter says hello
and ideally this would be a great place to put in our user story ...
but I won't do that right now ... just for brevity
let's ... have this greeter says ...
hello and this is also to show that ... something that
if you haven't used Cucumber outside of the ESaaS Engineering course then
... it's ... you know interesting to see Cucumber used not for Rails
... and it really is you can in principle be writing
Unit tests if you wanted to in cucumber I guess I should also mention is that
I think ... religiously sticking to process of the acceptance test and unit test cycle
is absolutely critical for managing software in coming from from distributed
teams
... just ... if you're trying to incorporate lots of things that people have
done
independently and they haven't been meeting as they can do in a in a single office
then getting everybody to sort of follow this you know Red Cucumber red RSpec
or should I say
Red acceptance red ... red unit test
ah, gosh you know you it there's all sorts of
levels; levels within levels. So let's do something so then given a Greeter ...
let's get in ...let's do ...
its when I send a greet message
... then I should see
"hello" like so and we'll do save, then out
and we'll run cucumber there and
yeah so you know you're familiar with ... cucumber
... they we go this is it just running by itself and this is what's lovely about the RSpec
book
is its got a whole series of examples where you're
just working with cucumber and RSpec and it gives you a much ...
I think ... a wonderful ... insight into all these things
I think we then need to have - don't we - it usually goes inside the ...
step definitions ... trying to sort of do it
... the step definitions again need to go
into a - so oh yes - can I just do it, we can do ... nano features ...
step definitions, I might have to create that
step_definitions ... greeter
steps it may complain now that I don't have the ...
no it's done, alright that's good so let's ... pop those in there
... so y'know we're starting off with our Cucumber we need to get that,
we need to ... implement those
let ... go in here
and say that so given that we have a
greeter to let's make ... let's make a a
greeter ... and just call it greeter new
like so. And then when I send it a greet message
so ... let's ... get rid of that there and ...
do, ... so let's have a message let's that
do that - two at symbols there - message is equal to
at greeter dot greet like so
and then finally we get down to here it then I should see
we'll get rid of the stuff in there
and say message
should equal
there we go; so this is we're actually
using RSpec syntax in there
greeting and we need to call this
here greeting okay so control X and
save my file no, yes! Ah, and are you going
to now filename to write? Ah okay so I'm maybe just going to need to go in here and quickly
cd ...
documents cd GitHub cd, we've
called this acceptance underscore units, cd
features and then we just need to create step
definitions, naughty nano, step
def-i-ni-tions like so
... try again right .. there we go
saved that out. Okay, so now if we run Cucumber ... we should get some different kinds of errors, we'll get some
some running things so we've got an uninitialized constant greeter
... there so what we need to do is get our ...
greeter into ... a Cucumber
and so then we get a basic error and I think actually it's great to go through
these sorts of errors here. We've got like unitialized constant greeter
so, you know, our Cucumber feature is referring to something called a greeter that it doesn't know anything about
... simple solution to that here is that we go into
our step definitions and look at our greeter steps
we need to have some sort of ...
reference to a greeter ... if
we get out of there ... that's still not gonna ... fix things for us
because we haven't got it's now going to require
a greeter; there's no such file ... following standard ...
Ruby practices we want to put ... something called
greeter dot rb in in there and we'll want to
... I was going to
not there you go and just creates a sort of default
greeter plus we could have dropped down with the ... there's a sort of
judgement call about the point at which you drop down to the lower-level unit
test but I think I just want to get -
you know, I know I need this infrastructure in place so if we now run
... Cucumber there ... increase the size of this a bit
we can see that ... we're now actually passing
the first step there ... which is ...
you know ... I've kinda cheated there a little bit ... to just go in and get us
something
... you know as a sort of a simpler, simpler error message but for now
on the second step we're getting undefined method greet so
we've got that but so we could of course carry-on and drive this
all the way through with with Cucumber and that's something that ...
is - is very tempting to do and this, you know, developing this intuition about when you drop
from
acceptance test to unit test is is kind of I think critical
for working ... on your code and producing reliable code which is then really
important for the - 
for the entire - for the entire team but so we can ...
... go; we can say like me maybe at this point I mean
we want to imagine you know all the functionality here is relatively relatively simple
you know we've just ... described it in in in nice language
what we want to do now ... is get set up with ...
... with some specs for our unit tests
so what I'm going to do here is if we make a spec directory
and we can run ... RSpec from the command line here and there's no examples at the moment
so if we go in and say ... nano
oh let's go, we're going to do spec and then do a greeter spec
... like so and then
... we can do something simple in here like we can describe well we'll probably need to
require
the greeter ... like this ...
and then we'll need to do you describe
... this greeter and say
... you know ... what shall we say? It's
... oh the interesting thing here is that as a unit test
rather than worrying about the high-level feature a bit sort of responding with
with the message
... you know it should respond
... to ... I think greeting I forget now what the error
was but let's - let's ... do that and
end and then I think we're got something like
the order of ... we've got ...
if we do greeter new
should respond to
and then ...greet. I forget if that was the right thing, well let's save that out
and was it was yes undefined method greet. so now let's run the RSpec there
and there we go; so expected Greeter to respond to greet
and it didn't ... so this is ... you can sort of see in this very trivial example that
we've got here if we go and look back at the ...
Cucumber example we've got here in the greeter feature
we've we've just described at the high level ...
you know ... given a greeter when I send the greet message
then I should see hello. We're sort of describing behaviour at a higher-level. We're kind of almost
doing kinda a bit of a
imperative thing here where we could sort of you know do fewer steps
... here that's another - another debate to get into.
but the key thing is about that we start with a higher-level description
you know potentially ... in a more human readable form ...
the ... you know that that's that's that's really important and then you know
at certain points we - we stop and we go down to the unit tests and the more simple
things like we've got
here we've got the spec and we've got the greeter spec and so now this is
arguably - still, you know - more - more human-readable in terms of the RSpec
greeter you should respond to to to greet. I wonder in fact if
I can get away ... with that just being ...
greeter I think probably if we had greeter should respond to greet
that's going to end up being the - the class method, anyway I won't get bogged down
in that now ... but so what we want to do then
... finally is ...
get over to our application code now that we've described the code,
the code we wish we had, at least we've described that it should respond to the greet method so
we're going to go nano
down to lib and our greeter and we'll go in here and we'll
add a method greet and we'll do
end there and control X out of that and let's see our our RSpec
... now passes but our Cucumber
will still fail I believe yes because
... now at least we've got one you know another one of our
cucumber steps as part of the high-level feature is not passing. Its expecting to see
hello
and we're not seeing hello and you can ... may be if we go back to the
slides this is this you know there's potentially many little unit test cycles
for this
these larger acceptance test ... cycles at the top level
particularly to the extent that we've broken up that acceptance test into those three
components ... but so those components almost ... almost that's the way it has been structured ...
corresponding to individual unit tests. So let's go and have a little another
unit test which is maybe that the default response should be hello. So if we go in here and we do nano
spec
... what's the next thing ... forgotten what it's called ... greeter spec like that
and then we could have another one where we say its ...
should respond with ...
hello ... how can I do it ... hello
by default ... and do
and then we can say a greeter
think that's right ... new
... and we've got greet ...
should equal
... hello just by default and we'll do
... and there save that and
so now let's see our spec. So we've got now a failure. One pass one failure there
Where this is another little unit test loop ... so
we can you know and if we happen to run I mean usually we wouldn't necess ... I mean
to the extent that we just only made changes to
... unit tests we wouldn't particularly need to run the acceptance tests ...
test ... the higher-level ... but so what I would do now is go into our
Ruby code there and just give this a default
... return value of hello like so
and we should see now that our unit test top, I've
you see, sometimes you have to go back there and
... let's just that like so. Like that
run the RSpec so that's now part of our all of our little
... individual unit tests are are passing
and if we come back up to cucumber we should see that that now all
goes green so there we go. That was this acceptance test unit test
... cycle in action I was using cucumber for the high level and
Rspec for the low level but I didn't have to I could have done
... you know, it with different tools I could've used RSpec for both of them
... the key thing I would say is that ...
you know you want to keep doing this over and over again religiously
... the RSpec book is is a great
... you know aid to sort of seeing that in low-level from a
lot of different perspectives and yeah this
you know this is of course the, I would say valuable to the to the solo individuals, to the
centralized team, to the distributed team
but particularly as regards the distributed team
where there may be ... the communication may not be as effective
as it is in a centralised team or as obviously you know within an individual's mind of course
that depends on the individual.
... you know you really want this kinda rigor
... to make sure that you're connecting what you're doing to the high level customer
story as business value
and then that all of the individual little elements are testing
and I can't say often enough its absolutely critical that you see
all of the tests fail before you see them pass. I often
get pull requests from from developers around the world
and you know great lots of fantastic tests but you know sometimes I can break
the
application and I see that the test does not fail and you know that that just
basically is is not what we want to see. Of course mutation testing
if we could automate that and add that into pull requests that would be very good but that's something
we're working on in Agile Ventures. Alright so that said the BDD/TDD cycle versus the
acceptance test
unit test cycle. My personal preference call it acceptance test unit test ...
but it is the way to Clean Code
Bye for now.
I think there's often confusion about what these are and the difference between them
I see them - I personally see them - as pretty much the same thing
... I would argue that maybe TDD is the bigger set
... and you know BDD is kinda a subset
of TDD ... the key thing you know and ... I'm not the
Oracle on this but seems to me that in order for something to be behaviour driven development
you need to have a higher level description of the expected behaviour
you need to have something that's that's ... comprehensible
to someone who doesn't know your code ... inside and out
... and so I mean I think the term Behaviour Driven Development was developed by the
people who
developed RSpec and Cucumber ... I think although that JBehave was the
original
precursor and I think the idea was to move away from the
... the test, ... I mean it's still you know Behaviour Driven Development still has this same sort of
flow
in that you know describe a behavior that you don't yet have
implement that behaviour ... you know ... see that - you know -
... that that's ... there's that in place
with the, ... it sorta, ... to test - Test Driven Development
is that same flow but the Behaviour Driven Development y'know, it says, right -
we can't just specify low-level tests we have to
specify the high-level behavior and so some tools in fact both
RSpec and Cucumber ... by their creators are suggested to be
BDD tools because they can describe things
at that, ... sort of a higher-level
now there's maybe some confusion that arises from this in the course
in that the 169 Engineering Software as a Service course
because we we ... breakup certain homeworks as we talk about the BDD
TDD cycle ... we have a homework which involves writing cucumber stories which
is
labelled a BDD homework we have ... the following
homework which is called BDD/TDD cycle which involves doing
both Cucumber and RSpec and I think one can come away with the impression that
somehow
"right ... oh yes cucumber is BDD RSpec is TDD"
that's what that's what happens ... and there are diagrams
that support this the you know and
you know I think the ... this concept is is around
so frequently that we can't kind of ignore it ... I feel
that it maybe ... I dunno it's not the most accurate way of
representing this. Whatever we call it, this process of having
... am higher-level feature tests and lower level, shall we call them, unit tests
... and sort of swapping from one to the other and going backwards and forwards
is extraordinarily powerful ...
in in some ways I don't get too wrapped up in the debate about what the
terminology, y'know how we describe it ... I think this
process with your centralized team of a distributed team
... you know even in your individual you know just this process of working
fundamentally can massively improve the quality of the software
that you that you generate. It's - it's not a - a magical elixir, but its - it really
really really can be a huge help and
you know we we're seeing that all the time in the y'know distributed teams
working on AgileVentures but just to go through you know as it's described in the
terms of BDD/TDD
the idea is that you would start by having a failing feature test
... there we've got the red arrows representing that so you got we've described sort of the high
level feature, the high-level behaviour that we want our software to have,
it doesn't have it. We would then rather then immediately making
that ... pass we would drop down to a low level and we would write
a lower level test ... that would also also be you know it was described here as
writing a failing test, a unit test
we see that fail. So then we're in this thing we have like two levels of red
above us; we've got a failing feature test
and then a failing unit test and then we will actually implement the code that we wish
we
we had and make that lower level test pass.
We would then refactor as we've ... heard talked about in the main course many
times
... and then ... ideally what will happen
is that as a consequence the ... high-level features test, because we've,
of course, done all our unit tests correctly, the high-level feature test ...
will will also pass ... of course there may be
you know it may be that ... for the high-level feature relying upon
several you know different individual unit tests that they might be
several several cycles there but ... and
well ... One: this is like I would say one the most powerful concepts
from from the course and in software engineering and I'm a big fan
... however I do worry about people calling it BDD/TDD cycle
... I prefer to call it acceptance test
unit test, or acceptance/unit test cycle let's talk about what we mean by acceptance
integration and unit tests
... particularly when I talk about these tests acceptance tests
coming from sort of an extreme programming background I'm talking about
just checking the entire stack, checking that there's the function you know all
of the functionality its present
I think depending upon where you're coming from that might be called system testing
and acceptance testing is when you actually put something in front of the
customer
... you know that ... I think again all of these terms
they're they're though the actual words; they're guides
like I think to get too hung up on what exactly
these things mean is to is to miss the wood for the trees ...
you know Wikipedia has a good article on all the different types of software testing
you know that's a - that's a - that's a great read ... but I I think
here what I want to do is try and ... focus on this -
this process and not get confused about ... you know
which tools go - go in where. Anyway listen - that's acceptance tests
which are kind of the higher-level tests and they are checking that things are really working
almost like from the perspective of the customer
.... then you ... sort of at a lower level down you have integration tests
that will be checking that ... a couple of different components in your system
are working well together and then unit tests being y'know single unit; that's checking
a single component
of your system and that give's us a diagram like this; there are many diagrams
out there ... I don't know that any of them are yet perfect we're still in search of ...
perhaps we will one day draw the perfect diagram, but
... you know I think rather than the
BDD/TDD, I think calling the top level
cycle of red/green/refactor the acceptance test cycle and the
smaller lower-level ... things the unit test cycles
they is is is better because the problem is that some people
... use RSpec to write their ... high-level feature tests
and ... you know although in the
... Engineering Software as a Service course we've used cucumber
for ... the behaviour ... sorry for the feature tests. I'm getting confused myself!
we've used ... cucumber for the high level and ...
RSpec for the for the lower level ... you don't have to do it that way round
I mean that you can argue that they lend themselves to those different levels
but it's not it's not required and so
... I think all this BDD/TDD is missing
the key point which is that you're you're ... whether you're using
... Cucumber or RSpec or even you're writing your own hand rolled framework
the key thing is that you have a high-level focus the you're
somehow attached to some ... user story or business value
right. And that there's some of ... you've got some sort of failing test
that represents that. Whether you're calling that you know
your feature test or you're calling it your acceptance test ... doesn't really matter
but the key thing is that you have that
and that that's your high level focus and
that you're then you know not relying solely on that but you're also
... testing the little components and the interfaces between them because your
high level tests will tend to run
rather slow and you can get ... you know
... it will tend to run rather slow and it may rely upon a whole cascade
of things and it's difficult to write tests for all of the different possible ways ...
the pathways through that. That's where your smaller y'know unit tests they allow
you to to focus on on a low level thing
but whenever you're working on a on your test you should be able to say what your
high level acceptance test is and often
people are asking me for help online; they're saying I've got this little tiny problem
here and it's stuck or it's not doing this thing
and I - the first thing I say is - the first thing I think is, actually, what I say is
you know ... what's the ... what's the chore or story that you're working on in the
bigger picture of the project, 'cause I want to understand that
and then I say right okay what's the acceptance test issue and then what's the unit test
issue
and the final we'll ... finally we'll look at whatever comes up
in the actual application code ... so this this is a pretty good diagram I
think
... it doesn't really show the flow from you know okay you've got an acceptance test cycle and its
you've got unit test cycles
embedded within it. It doesn't show about the
flow in quite the way that I wanted. This is another good - good
... diagram ... although because the arrows are not numbered
I think it can be ... somewhat confusing I think the way that its supposed to be
read is that you so start here
and ... on the top level here we've what you know top
circle or the outer circle with the acceptance test and you would initially have
a an acceptance test going red which might be in Cucumber, might be in RSpec but anyway
... you have that going red and then you would drop ... the first thing you do is you
drop down here. Now
failing acceptance test means it's now time to ...
have a failing unit test which you then make it pass and then you refactor
and then once you've got you know some number of unit tests
... passing sufficiently so who you think you've got all the ones that are part of this high-level
feature
you would then jump back out and hopefully see your high level acceptance test
pass and then you might do some refactoring there so this is this is a pretty
good diagram
I like this one I just yeah it needs numbers and an explanation to go with it
but this I believe is based upon what I would almost call the missing manual
y'know I think this
RSpec book ... which is all about RSpec and Cucumber
and friends is just excellent I couldn't I can't recommend it enough
... I think it's an excellent ... addition to the
Engineering Software as a Service textbook ... a lot of the material
from the RSpec book is in I think it's all there if you look it's it's all there
the ... this is I think such an important topic
that you know ... the way that it is presented
independently of Rails and you know Software as a Service and so on
... it's it's it's it's really really handy ...
but so that ... previous diagram - that comes from a diagram
from the the RSpec
... RSpec book which ... is the same, it doesn't have the colours but it does have the numbers so you can see
... this process here. It's a little bit of ... and it is the same thing
again but it's also got that if we look at it in
in text there ... so the and
... in the RSpec book as in the ... the ESaaS
course it ... the suggestion is to start to use cucumber as your higher-level testing
tool
... that's for features for acceptance tests and you know you you
focus on one scenario
you write a failing step definition. You drop down to,
you know, having done that you then drop down to RSpec you
write a failing example to get the example to pass. You refactor
and then you know go around around around and there's lots of excellent
... examples in the in the RSpec
book and you know I think the the challenge in some ways that we have with
the bigger ESaaS course with the
Rails and everything else that is being presented; it's
almost not until part 2 of the course that you actually get to practice
... this - this process ... and I was wondering I think I might just do
a little sort of concrete example of that on the command line; we'll see if and if this a
blows up in my face but if we wanna have ... just a simple
let's see. First I wanna do, so this is going to be I'm going to call this
`acceptance_unit` 'cause I wanna move away from BDD/TDD
let's go inside there and what I could possibly do is I could do
a features directory which we would ... need for cucumber
and then I could do something like ... nano
features ... now and I'm going to sort of adapt
... an example from the beginning of the RSpec
book here we'll call this ...
let's call this the greeter feature
... like so, there we go
and so we'll have a feature here that says
Greeter says hello
and ideally this would be a great place to put in our user story ...
but I won't do that right now ... just for brevity
let's ... have this greeter says ...
hello and this is also to show that ... something that
if you haven't used Cucumber outside of the ESaaS Engineering course then
... it's ... you know interesting to see Cucumber used not for Rails
... and it really is you can in principle be writing
Unit tests if you wanted to in cucumber I guess I should also mention is that
I think ... religiously sticking to process of the acceptance test and unit test cycle
is absolutely critical for managing software in coming from from distributed
teams
... just ... if you're trying to incorporate lots of things that people have
done
independently and they haven't been meeting as they can do in a in a single office
then getting everybody to sort of follow this you know Red Cucumber red RSpec
or should I say
Red acceptance red ... red unit test
ah, gosh you know you it there's all sorts of
levels; levels within levels. So let's do something so then given a Greeter ...
let's get in ...let's do ...
its when I send a greet message
... then I should see
"hello" like so and we'll do save, then out
and we'll run cucumber there and
yeah so you know you're familiar with ... cucumber
... they we go this is it just running by itself and this is what's lovely about the RSpec
book
is its got a whole series of examples where you're
just working with cucumber and RSpec and it gives you a much ...
I think ... a wonderful ... insight into all these things
I think we then need to have - don't we - it usually goes inside the ...
step definitions ... trying to sort of do it
... the step definitions again need to go
into a - so oh yes - can I just do it, we can do ... nano features ...
step definitions, I might have to create that
step_definitions ... greeter
steps it may complain now that I don't have the ...
no it's done, alright that's good so let's ... pop those in there
... so y'know we're starting off with our Cucumber we need to get that,
we need to ... implement those
let ... go in here
and say that so given that we have a
greeter to let's make ... let's make a a
greeter ... and just call it greeter new
like so. And then when I send it a greet message
so ... let's ... get rid of that there and ...
do, ... so let's have a message let's that
do that - two at symbols there - message is equal to
at greeter dot greet like so
and then finally we get down to here it then I should see
we'll get rid of the stuff in there
and say message
should equal
there we go; so this is we're actually
using RSpec syntax in there
greeting and we need to call this
here greeting okay so control X and
save my file no, yes! Ah, and are you going
to now filename to write? Ah okay so I'm maybe just going to need to go in here and quickly
cd ...
documents cd GitHub cd, we've
called this acceptance underscore units, cd
features and then we just need to create step
definitions, naughty nano, step
def-i-ni-tions like so
... try again right .. there we go
saved that out. Okay, so now if we run Cucumber ... we should get some different kinds of errors, we'll get some
some running things so we've got an uninitialised constant greeter
... there so what we need to do is get our ...
greeter into ... a Cucumber
and so then we get a basic error and I think actually it's great to go through
these sorts of errors here. We've got like unitialised constant greeter
so, you know, our Cucumber feature is referring to something called a greeter that it doesn't know anything about
... simple solution to that here is that we go into
our step definitions and look at our greeter steps
we need to have some sort of ...
reference to a greeter ... if
we get out of there ... that's still not gonna ... fix things for us
because we haven't got it's now going to require
a greeter; there's no such file ... following standard ...
Ruby practices we want to put ... something called
greeter dot rb in in there and we'll want to
... I was going to
not there you go and just creates a sort of default
greeter plus we could have dropped down with the ... there's a sort of
judgement call about the point at which you drop down to the lower level unit
test but I think I just want to get -
you know, I know I need this infrastructure in place so if we now run
... Cucumber there ... increase the size of this a bit
we can see that ... we're now actually passing
the first step there ... which is ...
you know ... I've kinda cheated there a little bit ... to just go in and get us
something
... you know as a sort of a simpler, simpler error message but for now
on the second step we're getting undefined method greet so
we've got that but so we could of course carry-on and drive this
all the way through with with Cucumber and that's something that ...
is - is very tempting to do and this, you know, developing this intuition about when you drop
from
acceptance test to unit test is is kind of I think critical
for working ... on your code and producing reliable code which is then really
important for the - 
for the entire - for the entire team but so we can ...
... go; we can say like me maybe at this point I mean
we want to imagine you know all the functionality here is relatively relatively simple
you know we've just ... described it in in in nice language
what we want to do now ... is get set up with ...
... with some specs for our unit tests
so what I'm going to do here is if we make a spec directory
and we can run ... RSpec from the command line here and there's no examples at the moment
so if we go in and say ... nano
oh let's go, we're going to do spec and then do a greeter spec
... like so and then
... we can do something simple in here like we can describe well we'll probably need to
require
the greeter ... like this ...
and then we'll need to do you describe
... this greeter and say
... you know ... what shall we say? It's
... oh the interesting thing here is that as a unit test
rather than worrying about the high-level feature a bit sort of responding with
with the message
... you know it should respond
... to ... I think greeting I forget now what the error
was but let's - let's ... do that and
end and then I think we're got something like
the order of ... we've got ...
if we do greeter new
should respond to
and then ...greet. I forget if that was the right thing, well let's save that out
and was it was yes undefined method greet. so now let's run the RSpec there
and there we go; so expected Greeter to respond to greet
and it didn't ... so this is ... you can sort of see in this very trivial example that
we've got here if we go and look back at the ...
Cucumber example we've got here in the greeter feature
we've we've just described at the high level ...
you know ... given a greeter when I send the greet message
then I should see hello. We're sort of describing behaviour at a higher-level. We're kind of almost
doing kinda a bit of a
imperative thing here where we could sort of you know do fewer steps
... here that's another - another debate to get into.
but the key thing is about that we start with a higher-level description
you know potentially ... in a more human readable form ...
the ... you know that that's that's that's really important and then you know
at certain points we - we stop and we go down to the unit tests and the more simple
things like we've got
here we've got the spec and we've got the greeter spec and so now this is
arguably - still, you know - more - more human-readable in terms of the RSpec
greeter you should respond to to to greet. I wonder in fact if
I can get away ... with that just being ...
greeter I think probably if we had greeter should respond to greet
that's going to end up being the - the class method, anyway I won't get bogged down
in that now ... but so what we want to do then
... finally is ...
get over to our application code now that we've described the code,
the code we wish we had, at least we've described that it should respond to the greet method so
we're going to go nano
down to lib and our greeter and we'll go in here and we'll
add a method greet and we'll do
end there and control X out of that and let's see our our RSpec
... now passes but our Cucumber
will still fail I believe yes because
... now at least we've got one you know another one of our
cucumber steps as part of the high-level feature is not passing. Its expecting to see
hello
and we're not seeing hello and you can ... may be if we go back to the
slides this is this you know there's potentially many little unit test cycles
for this
these larger acceptance test ... cycles at the top level
particularly to the extent that we've broken up that acceptance test into those three
components ... but so those components almost ... almost that's the way it has been structured ...
corresponding to individual unit tests. So let's go and have a little another
unit test which is maybe that the default response should be hello. So if we go in here and we do nano
spec
... what's the next thing ... forgotten what it's called ... greeter spec like that
and then we could have another one where we say its ...
should respond with ...
hello ... how can I do it ... hello
by default ... and do
and then we can say a greeter
think that's right ... new
... and we've got greet ...
should equal
... hello just by default and we'll do
... and there save that and
so now let's see our spec. So we've got now a failure. One pass one failure there
Where this is another little unit test loop ... so
we can you know and if we happen to run I mean usually we wouldn't necess ... I mean
to the extent that we just only made changes to
... unit tests we wouldn't particularly need to run the acceptance tests ...
test ... the higher-level ... but so what I would do now is go into our
Ruby code there and just give this a default
... return value of hello like so
and we should see now that our unit test top, I've
you see, sometimes you have to go back there and
... let's just that like so. Like that
run the RSpec so that's now part of our all of our little
... individual unit tests are are passing
and if we come back up to cucumber we should see that that now all
goes green so there we go. That was this acceptance test unit test
... cycle in action I was using cucumber for the high level and
Rspec for the low level but I didn't have to I could have done
... you know, it with different tools I could've used RSpec for both of them
... the key thing I would say is that ...
you know you want to keep doing this over and over again religiously
... the RSpec book is is a great
... you know aid to sort of seeing that in low-level from a
lot of different perspectives and yeah this
you know this is of course the, I would say valuable to the to the solo individuals, to the
centralized team, to the distributed team
but particularly as regards the distributed team
where there may be ... the communication may not be as effective
as it is in a centralised team or as obviously you know within an individual's mind of course
that depends on the individual.
... you know you really want this kinda rigor
... to make sure that you're connecting what you're doing to the high level customer
story as business value
and then that all of the individual little elements are testing
and I can't say often enough its absolutely critical that you see
all of the tests fail before you see them pass. I often
get pull requests from from developers around the world
and you know great lots of fantastic tests but you know sometimes I can break
the
application and I see that the test does not fail and you know that that just
basically is is not what we want to see. Of course mutation testing
if we could automate that and add that into pull requests that would be very good but that's something
we're working on in Agile Ventures. Alright so that said the BDD/TDD cycle versus the
acceptance test
unit test cycle. My personal preference call it acceptance test unit test ...
but it is the way to Clean Code
Bye for now.
