# Pragmatics of reference

The problem is to define reference.  I propose a definition that I
haven't seen previously.  I don't know whether that's because it's
new, or because it's wrong, vacuous, or foolish.

Reference is a mysterious relationship, because it seems to suggest a
word or phrase reaching up out of the page to some object "in the
world".  It is so unusual that it is usually left undefined.  Everyone
knows what it means but no one can say what it means.  It is even
taken as an undefinable primitive in IAO, an otherwise rigorous
information ontology.

The original motivation is the following question: Can we talk about
reference in specifying the language generation and understanding of
engineered artifacts (agents, computers, network endpoints, robots),
and if so, how?  Such talk has to be "hard nosed" in the sense that it
can be used in contracts, standards, and other potentially adversarial
contexts - so it cannot be "philosophical" or reliant on trust.

The question comes up in so-called 'knowledge engineering' contexts
such as the so-called 'semantic web', and I expect it to come up in
future scenarios involving communicating robots, e.g. what do two
somewhat-untrusting robots talk about when they meet on the sidewalk.

Of course the philosophical motivation of understanding the nature of
reference and compositional semantics is also strong; I'm not
satisfied with any of the conventional accounts (and there are whole
books written about reference).

The following is a bit of formalism intended to explain the core of
the idea.  Formalism is for people who appreciate the benefits and
limitations of formalisms.  If that's not you, please read something
else.  The formalism should not be mistaken for the idea itself, nor
should it be mistaken for an attempt at mathematics.

## The basic exposition

Assume an ordinary state-space framework, where the world is in
different states at different times (or along any other independent
variable). We can take the world W to be a set of world-states

    W = {ws1, ws2, ...}

A proposition p is a predicate over world-states:

    p  in  W -> Answer

where Answer = {true, false}.  (Isoontically, we could say p is a
subset of W, but it works out better to think of it as a mapping.)

Def. An object o is a pair <o_states, o_mapping> where o_states is a set of
object-states

    o_states = {os1, os2, ...}

o_mapping is a surjective mapping from W to o_states (making o_states
both the image and the range of o_mapping).

Def. A proposition p is *about* an object o if it factors through o,
i.e. there exists a function q from o_states to Answer (a predicate)
such that

    p(ws) = q(o_mapping(ws))

for all ws.  Equivalently: p is about o if its truth value is
determined by the state of o.

Let c be an object (a 'channel'), and call a state s of channel c a
'sentence'.

Say that a sentence s 'means' a proposition p if p(ws) is true in
those world-states in which the state of c is s (you might say: p if
and only if state(c) = s).

Suppose that each sentence s is composed of two parts, called sp and
vp, so s = <np, vp>.

Def. np refers to o iff every for every vp, the sentence <np, vp>
means a proposition that is about o.

## Application to engineered systems

This is a productive route, I believe, because it lends itself to
empirical study and engineering utility in a way that the usual talk
of "intention" and "representation" do not.  Here's how.

Meaning is empirical because it is experimentally falsifiable.  To
assess a claim that s means p, we can monitor the state of c, and each
time it is in state s, we can check to see whether p (i.e., whether p
of that world-state is true); if p is true, the claim is corroborated,
and if it is not, it is falsified.

Therefore, at worst, to determine meaning, we can run through every
world-state and record the relationship between the c-states and the
p-states (Answers).  That relationship is the meaning relationship.

In practice we may have more effective ways of assessing meaning, such
as asking questions of an agent that is controlling the state of c (s?
yes/no).  Then, we can run through all world states assaying whether s
is a 'possible' or 'sayable' state of c.  So it may be possible, in
principle, to determine meaning simply by observation.

I don't think that specifying or testing meaning is a problem.
Engineers to it all the time - they speak of the meaning of a signal
carried on a wire, or a message in a network protocol, without
difficulty.

What the above definition of reference does it to derive reference
from an oracle for meaning (any oracle).  Meaning is directly
testable; reference less so.  To challenge a claim that a
sentence-part np refers to an object o, look for a vp in which 
<np, vp> does _not_ mean a proposition that is about o.

How is a proposition p _not_ about an object o?  If p doesn't factor
through o - if its truth is sensitive to something other than the
state of o.  This can be detected empirically, by finding two world
states that are the same with respect to o (map to the same o-state),
but lead to opposite senses of p.

## Followons

I've written about most of these topics elsewhere, but want to list
them so that someone seeing only the above knows that there is much
more to the story.

Intuitively, we are really interested in whatever proposition,
independent of c, is coincident (co-true/false) with the proposition
that the channel is in state s.  The meaning of s is the former, not
the latter.  To get at this requires bringing in more apparatus
(agents? possible worlds? various lines of attack).

There is a connection betwee the part/whole relationship between
objects, and the is-about relationship, via the formalism (o' is part
of o if predicates over o factor through o').

Transitive verbs and relationships between objects (is a relationship
a proposition that is about a pair of objects?)

How verb phrases work in this setting - we expect them to 'mean'
prediates, through being generic over objects (implying that the
objects they're generic over are somehow similar to one another)

The propositions about an object form a boolean algebra.

Limitations on objects: they need some kind of internal logic or set
of correlations between their propositions-about, in order for us to
have compositional semantics and learnability.  An object can't be
just a bag of unrelated propositions, for example.

Above we have declarative meanings; to cover communication in
generally, need to cover imperative and combined
declarative/imperative meanings as well.

Is reference a functional relation?

Of course the apparatus of meaning is carried by a population of
agents via their behaviors of generation and interpretation.

Evolutionary game theory (or economics) of agents - benefits of
communication ('information transfer') - fidelity vs. cheating.

## References

A good chunk of this comes from Yablo's book _Aboutness_.

There's a big literature on intentionality, including Brian Cantwell
Smith (who got me started on this question), but I don't know whether
or how it's relevant.

