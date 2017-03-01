#Functional Programming Inception

[Alexandru Nedelcu (alexelcu)](http://twitter.com/alexelcu)

[https://alexn.org](https://alexn.org)

Eloquentix + Typelevel

## Abstract

Designing functionality that exhibits the properties of functional programming is hard because it requires a mentality change, coping with immutability and consideration for recursivity, performance and polymorphism. This talk is a lesson in FP design that makes use of Scala’s hybrid OOP+FP nature.

## Description

Designing functionality that exhibits the properties of functional programming is hard because it requires a mentality change, coping with immutability and consideration for recursivity, performance and polymorphism. This talk is a lesson in FP design that makes use of Scala's hybrid OOP+FP nature.

We are going to start from Scala's (and Java's) ubiquitous `Iterator`/`Iterable` types which expose the famous iterator pattern, analyzing its strengths and weaknesses. And then we are going to work your way up to a fully featured FP replacement that has referential transparency and that fixes everything that's wrong with iterator, while being more generic.

This lesson in design involves talking about immutability, imperative programming, asynchrony and problems encountered when going FP, like performance considerations or recursivity. We are also going to talk about ADTs, higher kinded polymorphism and type-classes versus OOP subtyping. Interestingly the example presented will use both OOP subtyping and type-classes and thus we can make a clear comparison about what to use and when - a problem that the Scala developer has in his daily work.

A working knowledge of the Scala programming language is required. Knowledge about Scala's `Future` or the `Task` data type in [Monix](https://monix.io/docs/2x/eval/task.html) or from Scalaz is recommended, but not required.

## Notes

Hi folks,

I'm Alexandru Nedelcu, [@alexandru](https://github.com/alexandru) on GitHub/Gitter and [@alexelcu](https://twitter.com/alexelcu) on Twitter, the lead developer of the [Monix](https://monix.io) library. 

Links:

- [alexn.org](https://alexn.org) (personal blog)
- [monix.io](https://monix.io)

Cheers,

## Bio
  
Alexandru is a software developer living in Bucharest, Romania, currently working for Eloquentix. A startup guy, by day he's been helping with projects for powering the next generation energy grid solutions and for advancing the health-care industry. By night he's fueled by his work on the Monix project, the Scala library for composing asynchronous and event-based programs. He's also a proud father, husband, has a very unhealthy sleep schedule and appreciates talking about programming over beer. Sometimes he blogs at: https://alexn.org