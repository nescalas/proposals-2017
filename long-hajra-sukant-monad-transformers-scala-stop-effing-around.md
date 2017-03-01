#Monad Transformers: Scala, stop Eff'ing around!

[Sukant Hajra (shajra)](http://twitter.com/shajra)

[http://github.com/shajra](http://github.com/shajra)

Cognitive Scale

## Abstract

Stop chasing Eff'ing Free Cakes with classy optics for a moment, and smell the monad transformers.

All you wanted was an FP solution to dependency injection and error handling, right?

Let's see how far we can get with monad transformers before leaping to the next thing.  You may need nothing more.

## Description

With the fairly consistent stream of new Scala developers, it's still common to have to answer the question of "how do I do 'dependency injection' with pure FP in Scala?"  Over the years, there have been a slew of talks about this from the Cake pattern to Free monads, often with only a short pit-stop at the Reader monad.

But eventually the thoughtful typesafe functional programmer wants to stop throwing exceptions everywhere, and we find ourself reaching for tools like the EitherT monad transformer.  And we might realize that even with a Free monad, we still need to write an interpreter.  So we've delayed the original problem, but not really addressed it.

Finally, someone might mention using a stack of monad transformers.  But it seems very popular these days for Scala developers to balk at syntactic and type inference inconveniences.  This recently has lead to variations of Eff from the _Extensible Effects_ paper.  However, this approach comes at a cost of correctness.

This talk attempts to do what I think we should have done a while ago -- see how far we can get in Scala with monad transformers a simplier way, with a touch of parametric polymorphism and perhaps a hint of optics.  With monad transformers, less is more.  We want to use parametric polymorphism to hide the complexity of the transformers.  Otherwise, we'll run into syntax and type inference woes.

Abstractions are beautiful, but let's make sure to fully explore the ones we have already, so we can more reasonably assess the next idea to come along.

Type systems are wonderful, but let's not forget about simplicity.

## Notes

My goal is to get people to consider how far we can go with the following type:

```
[M : ComponentA : ComponentB : MonadIO]: EitherT[ErrorADT, M, ?]
```

`ComponentA` and `ComponentB` will be domain-oriented interfaces, like `Database` or `Logging`.  This is exactly how the Java programmer thinks about "dependency injection," except they use an unsafe object-oriented melange of dynamic dispatch and reflection.  We'll take their intuition of what a good interface is, but use the static dispatch of type classes instead.

There may be a need for supporting code that doesn't yet exist in Scalaz or Cats.  And the state of effect tracking types is still a bit of a mess.  But this is more of an exercise in proving a point, and also of establishing a pattern of using monad transformers in Scala that isn't crippled by type inference woes.  It will be backed by real code that compiles and runs, but more work may be needed to have enough combinators for production code.

I've been doing this style of programming in Haskell for a bit now, and it struck me that I've never seen this done in Scala.  I'm not sure why.  But I'd like to see if I can fix that.

## Bio
  
Since 2010, I've been using the kind of type-checked FP that restricts programs to math-like total functions (as exclusively as I've known how).  I started doing this first for a government project in Java, which was feasible, but a touch verbose.  I switched to Scala shortly there after while working at Rackspace.  Recently, I've been using Haskell professionally, orchestrating machine learning algorithms for my current employer Cognitive Scale.  I also help advocate for type-checked FP in my home town of Austin, organizing both our Scala and Haskell meetups.

I'm not sure these are the greatest reasons for someone to listen to me.  I just care about doing this stuff well, because it seems like too much software breaks a lot and is hard to work with.