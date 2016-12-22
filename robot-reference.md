
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

I'm going to focus on subject phrases (or noun phrases), of which
names and nouns are special cases, for a number of reasons.

1. Every known (compositional) language, whether natural or
artificial, has sentences composed of a subject phrases and a
predicate phrase.  [I guess I need to back up this claim.]  I do not
know whether a language lacking them could exist, but their importance
is important simply on the basis of evidence.

2. One must start somewhere; we could start with predicate phrases
instead.  But the choice could be arbitrary.  (I have a feeling it is
not; that it is logically more natural to understand predicate phrases
once subject phrases are understood.  But that should become clear if
the analysis gets far enough.)

When we try to characterize the role of subject phrases in behavior,
we inevitably talk of the independent role of the subject phrase as
being _referring_.

