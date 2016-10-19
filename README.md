WORK IN PROGRESS - SUBJECT TO REVISION WITHOUT NOTICE

# Communication

## Communication system

A communication system consists of agents connected by channels.  The state of a channel is called a sentence (or message), i.e. a channel carries different sentences at different times.  The state of a channel is controlled by one or more agents, and sensed by one or more agents.

When an agent causes a particular sentence to become the state of a channel, it is "generating" the sentence.  When an agent senses the state of a channel and acts contingently on that sentence, it is "interpreting" the sentence.  Agent A generating S on C, followed by agent B interpreting S on C, is a "communication event".

Every channel has a quiescent state, i.e. one in which no generation is happening.

* I don't say that 'communication system' is an ontological category. It could be more of a role or an analytical structure, i.e. we look at the world and call out a few entities as being a 'communication system' in order to help begin and structure a discussion about them.  In any case, if we don't have agents controlling and sensing a channel, we don't have a communication system.
* I'm not prepared to define 'communication' and I'm not sure I need to.
* By 'generate' and 'interpret' I mean to imply the agents' _involvement_ in selecting the sentence and choosing how to respond - not just in proximally relaying or transducing the channel state.  A speaker or microphone, or mail carrier, is not generating or interpreting.

## Meaning

A sentence S (on a given channel) means the proposition P, where P = P1 AND LATER(P2); P1, generally speaking, is what holds when an agent generates S; and P2 is what holds after an agent interprets S, generally speaking.

* LATER is a modal operator similar to the deontic OB: LATER(P2) iff an interpreting agent will bring about P2.
* "Generally speaking" means we are talking about what is common to many communication events on a channel in a system, not any particular communication event.  We can't talk about this kind of "meaning" except as a generalization about the behavior over time of a communication system.
* We could talk about "generally" as implying that the meaning of a sentence is a statistical property of a system, although I'd rather not (I note that people usually do not do so, in ordinary conversation).
* This use of "meaning" coincides with one common use, but the word gets used in many other ways (including within this page!).  That might argue for qualifying it somehow, or using a different word.
* If P2 is empty - that is, nothing generally seems to hold when S is interpreted - we say that S is 'declarative'.
* If P1 is empty - that is, nothing generally seems to hold when S is generated - we say that S is 'imperative'.
* See following for 'proposition'.

## Proposition

Something that can be true or false; a potential object of a propositional attitude.

* Just as a color-quality or color-variable (e.g. the color of the wall) can change over time but is a particular color at any given time, a proposition can vary over time but is a particular truth value (true or false) at any given time.

## Truth and fidelity

Individual agent actions can have a 'payoff' for that agent. If the payoffs are +/+ (positive for the generator, positive for the interpreter), the agents are acting cooperatively: the generator is 'telling the truth' and the interpreter is acting with 'fidelity'.

(Assume that neither agent can get a nonzero payoff unless both generation and interpretation are taking place.)

If the payoffs are +/-, one might say that the generator has 'lied' to the interpreter, and if the payoffs are -/+, one might say the interpreter has 'betrayed' the generator.

One expects an agent to modulate its actions to maximize payoffs, integrated over time. In a communication system, the actions are generation and interpretation.  If the payoff to either agent is negative, that agent may stop generating or interpreting.  Since it takes two agents for there to be any payoff, the system will cease to be a communication system.

* What is a payoff?  In a biological setting, it might be an increment to fitness; in a commercial setting, it might be an exchange of money.  Over the long run, payoffs determine the phenotype and fitness of organisms, or design and production of goods.
* The payoff to the generator is going to be indirect through a causal chain, not involving the channel, beginning with whatever change the interpreter brought about to its environment and ending with some local state that the generator senses and 'likes' or not (payoff); similarly the payoff to the interpreter will involve a causal chain, not involving the channel, from whatever the generator sensed in its environment to some local state the interpreter 'likes' or not.
* Mistakes can look like lies or betrayals. That's what apologies are for. But as mistakes are 'unintentional', one would expect a lower payoff for a mistake than for a lie or betrayal.

## Compositional semantics

A sentence can have parts, in the sense that there are patterns to how the parts are used - the parts have "meaning".  Parts can themselves have parts, down to atomic units that one might call "words". Determining the part-whole structure of a sentence is called 'parsing'.

"Compitional semantics" refers to the ability of agents to use part-meanings (whatever those may be) to generate and interpret sentences with which they have no previous experience.

Empirically speaking, in both natural and artificial languages, an important observed pattern is elementary sentences consisting of two parts, a noun phrase and a verb phrase.

The (truth of the) meaning of a sentence reflects the agents' world.  If we "knew" the "language" of the agents, we might say informally that the noun phrase in an elementary sentence has something to do with some part of that world.  We might call this "has something to do with" relationship "reference" without knowing exactly why we do so. But is there an objective way to assess whether or not a given noun phrase refers to a given part of the agents' world, so that we can make judgments of reference without having to "know" the "language"?

## Reference

A noun phrase N refers to object O if every sentence whose subject is N means a proposition that is about O.

* For 'about' see below.
* This claim (or maybe it's a 'slogan', or a definition) is a general claim about a given system, not about particular communication events.
* 'Subject' here means grammatical subject, i.e. a part of the sentence.
* 'Object' is used with reluctance. It means roughly 'part of the world' (which depends on what 'part' means). It might be better to say 'refers to O' without saying anything about O.

## Aboutness

A proposition P is about an object O if its truth is sensitive to the state of O.  That is, P is about O if there is (hypothetically) some change that could be made to O that would change the truth of P.

* This definition relies on the ability to delimit the state of a given object.  Internal state such as hunger or temperature is pretty clearly state, but relations such as what one's wearing, position (with respect to the world), and ownership (is what I own part of my state, and am I part of its state?) are less clear.
* 'Change' and 'state' are clearly closely related, perhaps even interdefinable.
* Sometimes, as in IAO or Brian Smith's work, the term 'is about' relates sentences or sentence parts to objects, not propositions to objects.  My use is closer to Yablo's.

