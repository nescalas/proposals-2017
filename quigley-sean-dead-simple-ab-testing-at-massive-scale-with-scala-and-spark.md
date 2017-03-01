#Dead simple AB testing at Massive Scale with Scala and Spark

[Sean Quigley (s_quigls)](http://twitter.com/s_quigls)

[https://github.com/seanpquig](https://github.com/seanpquig)

GIPHY

## Abstract

As a small engineering team, GIPHY needs creative, lightweight solutions to deliver features for a massive global user base. Leveraging the type-safety and expressiveness of Scala along with the performance of Spark allowed us to rapidly deliver a reliable AB testing solution for our search engine.

## Description

Demand for richer content in messaging and internet communication continues to grow rapidly. As a provider of such content, GIPHY has seen exceptional growth in traffic while maintaining a relatively small engineering team. Engineering problems must be approached with the following constraints in mind:

- solutions must be designed to scale
- features need to be delivered as quickly as possible
- unnecessary architectural complications and dependencies on other teams need to minimized
- code should be as generic and extensible as possible

Search is core to GIPHY and we needed to better incorporate data into our feature decision-making process. AB + Multivariate testing was an obvious capability. This talk will cover how we designed such a solution within the above-mentioned constraints and why Scala was a natural choice.  Highlights include:

- parsing and modeling your data for use with functional paradigms in mind
- abstracting user experiments and statistical attribution in a generic and immutable manner
- maximizing Spark code reliability with compile-time safety and unit-testing
- adopting Bayesian inference over more classical frequentist approaches to empower more intuitive interpretations of experiments
- how a monorepo approach enables better code reuse and unification of services code with offline analytics


## Notes

This talk is designed for a range of audiences and experience levels.  Familiarities with functional-programming principles, big data architectures + Spark, and statistics relevant to AB testing are useful.

As a heavy user of Spark for the last couple years, I'm very familiar with how the APIs and engine have evolved and the powerful unification of type-safety and performance optimizations in the latest Dataset API.  I'm also a passionate Scala enthusiast and love how it provides a very advanced type-system and functional abstractions with the practicality of the JVM platform, a rock-solid, high-performance, library rich ecosystem. I love sharing how these features of Scala can empower very elegant, yet pragmatic solutions.

## Bio
  
Sean Quigley has always been fascinated with the abstract process of solving logical problems. This seems to be the one common theme on his journey from a fondness for math and puzzles as a child, to studying Physics and Economics at the University of Michigan, working as a hedge-fund quant, a data scientist in Ad-tech, and now a software engineer developing solutions for web-scale analytics and search at GIPHY. In his spare time, he enjoys martial arts, electronic music, and traveling.