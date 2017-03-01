#Using recursive typeclasses to model your data

[Thurston Sandberg (thurstonsand)](http://twitter.com/thurstonsand)

[https://github.com/thurstonsand/](https://github.com/thurstonsand/)

IBM

## Abstract

Combine implicits, typeclasses, and the Shapeless library's HList to create a powerful data model for anything that can be mapped to case classes. Recursive typeclasses can describe behavior such as SQL statements and json serialization/deserialization with minimal boilerplate and a succinct syntax.

## Description

### Learn by example

Using an easy to understand example, Scala's own Ordering typeclass, listeners will have a familiar point on which to learn, which helps makes this talk open for all skill levels, even for those that are previously unfamiliar with the Shapeless library. By focusing on this example, this talk stays compact and provides theoretical concepts and their implementations side-by-side.

### Building on core concepts to create something cool

This talk builds up an understanding of implicits, typeclasses, and Shapeless's HList, so that listeners understand the deep mechanics by which recursive typeclasses work. By showing the actual inductive (and recursive) steps that occur when building a recursive typeclass, this talk will help listeners come to grips with a lot of the magic that occurs when using Shapeless's HList and the compiler's implicit function resolution.

### Real-World Application

This talk was created in response to the many lessons I learned while writing an open source library that creates a Scala interface to Cassandra using the existing Java driver. [You can view that library here](https://github.com/thurstonsand/scala-cass) if you are interested in seeing one instance of how recursive typeclasses can be used.

## Notes

### Technical Requirements

I'm not 100% sure on whether you mean my technical requirements, or the technical requirements listeners will need to understand this talk, so I will list both.

#### My Technical Requirements

I will only need a projector and a place to plugin my macbook via either HDMI or thunderbolt.

#### Audience Technical Requirements

This talk aspires to be open to all, regardless of Scala experience. The first few slides will cover the topics of implicits, typeclasses, and case classes so that anyone can attend. While the application of Shapeless is rarely a beginner's topic, I focus only on the pieces of the HList that I need, and explain what they are with the hopes that anyone can understand its core advantages and uses.

### Why Me?

I have been working on a library that uses recursive typeclasses to interact with Cassandra. By wrapping over the Java Cassandra driver, I create a Scala interface that can model tables as case classes to allow for selects, inserts, deletes, etc. [Here is a link to that open source library](https://github.com/thurstonsand/scala-cass).

I have also recently given this talk at a local Scala meetup, and have the presentation available with full speaker notes [here](https://docs.google.com/presentation/d/1U-KAHiwLDfiU2Ob2MyyMSyhT5-ZNzqLfVuLrU5VVbzk/edit?usp=sharing), although I do reserve the right to make some modifications to the presentation.

## Bio
  
I'm (relatively) new to the Scala scene, joining The Weather Channel mid-2015 straight out of Georgia Tech and learning Scala on the job. Since then, I've fallen in love with the Scala language and its community, frequently trawling the gitter channel for useful insights and, sometimes, if I'm feeling confident, trying to contribute to the conversation myself.