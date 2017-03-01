#Recursion schemes and fixed point data types

[Arthur Kushka (arhelmus)](http://twitter.com/arhelmus)

[http://archdev.me](http://archdev.me)

AutoScout24

## Abstract

Its always a challenge to build a good abstraction during work on library. Recursion schemes its a perfect way to reduce complexity of codebase and provide readable, tree-like interface for your customers.

## Description

Its always challenge to build a good abstraction during work on library. Library codebase must be flexible and modular when user code must be clean and easy understandable. One of variants to build API between library and customer its Free evaluation approach. In that case you as developer is free to interpret customer actions as you want and customer is free to define actions as he want. In my talk I will show how to build API based on recursive abstract data types, describe why its cool and demonstrate some tricks on type system to make customer experience with library better.

## Notes

In WIX.com I worked on small internal library for event sourcing. One of the biggest challenges for me was implementation of search on denormalised datasets. Its quite easy to just put all data to elastic and give to customers elastic query builder, but... If you want to write really cool library, it must be modular without strict dependencies on other components. In my implementation with recursive ADT user may know only simple tree-like structure to define a query, all other things was done on library level. Also recursive ADT can be interpreted to any result query as elastic/sphinx and so on. During my work I found that a lot of boilerplate code related to recursive schemes already implemented in Matreshka library so I will show all my examples with it. As a result of my work, customers can forget about indexing engine that they use and library developers can interpret user actions as they want.

## Bio
  
Talented engineer that uses JVM stack for developing of great services and web applications. Prefers the functional design of code. Breathe life into ideas.