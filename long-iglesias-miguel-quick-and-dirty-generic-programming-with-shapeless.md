#Quick and dirty generic programming with shapeless

[Miguel Iglesias (caente)](http://twitter.com/caente)

[http://caente.github.io/](http://caente.github.io/)

x.ai

## Abstract

I will show how to make functions that would take any random number of arguments, and return an aggregated response for any *combination* of arguments for which the function is defined.

## Description

If you want to make Scala even _more_ confusing and awesome, read on:

In this talk we'll learn how to write a "function" that will take an arbitrary context -- i.e. a list of arguments -- and return _all_ the results that apply to any combination of the arguments.

e.g.
```
"word".functions(1,"a",2d) === List(5, 10)
```
Each element of the resulting `List` is a result of an argument  _combination_ -- i.e. the first is because `1` and `2d` and the second because `2d`. The `"a"` is ignored.

We'll achieve that using shapeless and type classes. It really is "simple" -- abstract -- and fun.



## Notes

This talk is from an actual use case at work. We shouldn't need this, but that's life, we needed it and scala+shapeless made it possible. The looks of incredulity of my coworkers was so awesome, and I had so much fun implementing this, that I thought it would be a good subject for a talk.

## Bio
  
I've been a back-end engineer at x.ai for two years, focusing mostly on how our robot interacts with the customer; in other words, I've been selfish and stayed on the fun part of the job :-)
I push my self towards simplicity, but won't shy away from complex/weird methods to achieve it. 
I basically try to keep my mind constantly blown, not a hard thing to do once you find functional programming.