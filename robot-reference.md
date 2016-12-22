
Robots are of interest as components of engineered systems, as goods
that are traded commercially, and as fellows sharing our physical and
social spaces.  We care about how they will behave and what they will
do.  _Specification_ is simply the act of being specific about
behavior: either attesting to a prediction or promise of what
something will do, or requesting that it should do something specific.
Robot specifications therefore ought to be of great interest, and
should be of increasing interest as robots become more capable and are
entrusted with increasingly important tasks.

Someone who says that a specification will hold can be held
accountable for the robot's actions, increasing our confidence in the
robot.  This is why specifications are central to engineering and
commercial transactions: they can be used to create socially
consequential agreements between robot users and robot providers (or
between buyers and sellers), even when the parties are suspicious of
one another.  A specification protects the provider from unreasonable
expectations on the part of the user, and protects the user from
having the provider deny that the user is entitled to a particular
behavior from the robot.

One thing that robots do is to communicate.  It follows that we should
care what they say, and what they do in response to what is said, and
that we should want these things to be specified.  One might start
with: When the robot sees a walnut, it says "walnut".  This can be
made as specific as one likes, by clarifying (between provider and
user) what is and isn't to be considered a walnut, what sort of
lighting and environmental conditions are required before one can
expect this behavior, and so on.

Generalizing a bit, we might have a number of "sentences" similar to
"walnut" in that some particular sensation or behavior is associated
with each one.  A system of such sentences with associated behavior is
called a signalling system.  Signalling systems are well studied, from
animal systems such as vervet monkeys to Shannon's theory of
information.  One can go a long way with such a framework.

Ordinarily, one speaks of _meaning_ rather than behavior, but this is
just a grammatical rearrangement; the effect is the same.  Instead of
specifying that "when the robot hears X it will do Y" or "the robot
will only say X when Y holds", we can express the same constraints as
"X will (or must) means to do Y" and "X means that Y", and no one will
be confused.  _Meaning_ makes perfect sense in a specification because
it implies conditions that can be tested, i.e. conditions that the
provider can be held to (or not, as the case may be).

Signalling systems are powerful as far as they go, and account well
for elementary communication patterns, but they fail to account for
_language_.  Language goes beyond mere communication in that it is
_compositional:_ a speaker can create new sentences by combining
smaller phrases, and still have them be understood - even though the
speaker may never have said that sentence, and the listener has never
previously heard it.

Compositionality radically advances communication.  For this reason it
is important to be able to specify robot behavior that relies on
linguistic composition.  But how to do that is not obvious.  If a
robot says (or hears) the sentence 'P1 P2' where P1 and P2 are
phrases, we should have certain expectations of the robot's behavior -
but what?  The way in which P1 being part of the sentence relates to
the robot's behavior depends on what P2 is, and vice versa.  This does
not sound impossible, but it is puzzling, at least.

I'm going to focus first on subject phrases (or noun phrases), of
which names and nouns are special cases.  Every known (compositional)
language, whether natural or artificial, has sentences composed of a
subject phrases and a predicate phrase.  [I guess I need to back up
this claim.]  I do not know whether a language lacking them could
exist, but their importance is important simply on the basis of
evidence.

We could start with predicate phrases, or other sentence structures,
instead.  Take the choice of subject phrases as parts of
subject/predicate phrase sentences as arbitrary for now.

The problem now is what kinds of things we might say in order to
specify the relationship between robot behavior (or let us say 'agent
behavior') and compositional subject phrases occurring in message
heard and said by the robot.

We have two precedents to examine: artificial language and natural
language.

Artificial languages are designed for instructing a computer on what
it ought to do, i.e. programming languages.  The linguistic behavior
specification in question is that for the software responsible for
interpreting the artificial language.

Natural language is used for communication between people, and to a
very limited extent between people and computers.  Here we are not
_engineering_ the humans so we do not talk about specifications so
much.  Rather we are trying to _understand_ how humans do what they do
with language, and seek scientific _descriptions_ of their behavior.
Descriptions and specifications look the same, and are only
distinguished by what one does with them, so good descriptions should
tell us what good specifications could be like.

ways in which artificial languages fail:

1. According to the programming language documentation, subject
phrases relate ("refer") to entities in the computer's address space,
not to entities in the world.  When we use a robot, properties of the
address space are only indirectly relevant to what the robot does, so
they are not what we really care about.

2. Programmers clearly have in mind that certain data structure
"represent" or are "proxies" for things outside the address space.
For example, an `employee` record may have `name` and `year_of_birth`
fields.  The tokens (as natural language) are obviously chosen to be
suggestive, and lead one to suppose a set of relationships: the
`employee` record might bear some relationship to an employee of a
business, its `name` field might have some relationship to that
employee's name, and so on.  In a well documented program these
relationships will be spelled out, but obviously that documentation,
written in natural language, is not affecting what the computer does.
Any solid information we have about these relationships (where the
values come from, when and how it gets corrected, and so on) relates
to the larger system in which the program is embedded.  That larger
system involves the computer, the employee, those doing data entry,
company policy, and so on.

Artificial languages do not help us much here.  Computer programs
relate only to the computer's role as a component of a larger system.
These systems typically rely on people in order to learn about and have
an effect on the world.  They do not run autonomously or possess
independent non-linguistic knowledge or control of their environment,
as we expect robots to.  A computer can wield huge amounts of
information, but it is left to humans to interpret it.  Specifying
anything about a program only tells about narrowly about the computer
running the program; it says nothing about the real system we will be
interacting with.

ok.

Natural language, on the other hand, is clearly very successful in
having a finely orchestrated connection between composed linguistic
parts and arbitrary aspects of the world and behavior.  The difficulty
is that it is difficult to make operational (in a sense that would
satisfy a robot) the advice that usually passes for description or
specification.

Consider:

>    'Chicago' refers to the area under the jurisdiction of the Chicago
>    Metropolitan Agency for Planning.

This specifies that it would be incorrect to use 'Chicago' to refer to
something else, e.g. the City of Chicago.  Like 'meaning' (above),
this specification is a cryptic constraint on the robot:

>    The robot must interpret 'Chicago' to be the area under the
>    jurisdiction of the Chicago Metropolitan Agency for Planning, and
>    must use it only to refer to that area.

Now suppose that we were a quality control engineer for this robot.
What would we do to test its conformance with this specification?

(not the best example since the robot has no sensors to detect
properties of Chicago.  fix.)

You can ask the robot questions, as if it were a student in a civics
class, probing not only what it "knows", but what it rejects.

