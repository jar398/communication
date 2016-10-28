
# Introduction

Two objectives here

1. Philosophers have been trying to understand meaning - by which I
mean, roughly, the relationship between what is said and the world -
for millenia, without a lot of success in my opinion.  It is my belief
that a study of at meaning in engineering contexts can shed light on
questions that to date have been in the domain of philosophy.  

1. The role of automated agents (robots, "internetworked things", and
so on) in society is transforming rapidly. As more of these devices
are created, and their capabilities expand, two things will happen:
their linguistic competence will increase, and the specification and
correctness of all their competences will become more important.  Who
wants to buy or use a robot whose communication is perpetually
suspect?  I believe that a theory of meaning in engineering contexts
can promote the trustworthiness and interoperability of robots, and
therefore increase their practical and economic value.

What I will do is to analyze communication and meaning the way an
engineer would, using state space analyses and verifiable system
properties.  The goal is to shed light both on the specification and
design of engineered agents, and on questions of human communication
that have confused the philosophers.

## Backstory

This project grew out of accumulating frustration.  In a series of
practical projects, the results were not as they could have been, for
want of a theory of meaning.

*Robot programming.*  
The natural approach to programming a robot, using easily available
tools, is what I would call 'solipsistic'.  Everything one says in the
program that controls the robot is in terms of the robot: one does
calculations and inference on sensor readings, actuator parameters,
and internal state (memory).  Yet these things are really of no
interest to someone trying to use or interact with the robot, and
therefore of litte use in communication.  The 'objects' of interest in
programming and communicating with the robot ought to be things in the
world, or aspects of the world, not things in the robot.  There are ad
hoc solutions in particular cases, such as reading a bar code or the
use of 'machine learning', but no principles.  How to properly bring
this about this 'aboutness' has been baffling.

*Knowledge representation.*  
Biomedical triple store ontologies etc.

*Semantic web.*  
The idea that we might construct a globally distributed "knowledge
base" or "knowledge graph" goes back to TimBL's 1989 paper.  The
project ramped up in the early 2000s and has proceeded in an organic
fashion since then without any engineering discipline.  That is, there
is no way to know whether one is participating correctly in the
process, because there is no notion of 'correct'.  In particular, some
of the tokens in the graph are said to 'refer to things in the world',
but without any actionable definition of 'refer'.  Lack of standards
and theory hinders investment in this enterprise.  When challenged on
how to test 'reference' TimBL said "you figure it out".  I tried for
six years and failed.
