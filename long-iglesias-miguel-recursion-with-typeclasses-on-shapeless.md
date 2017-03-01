#Recursion with typesclasses on shapeless

[Miguel Iglesias (caente)](http://twitter.com/caente)

[http://caente.github.io/](http://caente.github.io/)

x.ai

## Abstract

Shapeless bread and butter is compile time recursion with typeclasses. In this talk I'll explain how I gain intuition to reason about it.

## Description

I'll show how to write `Find[L,A]`, where `L` is an `HList`, which, similarly to `List[A](...).find(f: A => Boolean)`, will return `Some[A]` if it has a value of type `A`, but `None` otherwise:

```scala
("a" :: 1 :: HNil).find[Int] === Some(1)
("a" :: 1 :: HNil).find[Double] === None
```



## Notes

`Find[L,A]` is a typeclass that I thought I would never need, but software industry is full of uncertainties, and some times you do need an `Option[A]`.

## Bio
  
I've been a back-end engineer at x.ai for two years, focusing mostly on how our robot interacts with the customer; I've been selfish and stayed on the fun part of the job :-)
I push my self towards simplicity, but won't shy away from complex/weird methods to achieve it. 
I try to keep my mind constantly blown, not a hard thing to do once you find functional programming.
