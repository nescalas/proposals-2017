#Don’t Cheat the Executor -- Execution Contexts in Scala

[Scott Underwood (scottyunderwear)](http://twitter.com/scottyunderwear)

[http://underwood.nyc](http://underwood.nyc)

Troops.AI

## Abstract

Execution Contexts provide the means to execute program logic asynchronously, and are a prerequisite for using Futures and Promises. This talk will explore common mistakes in using Execution Contexts, and strategies for configuring, debugging and monitoring them and their underlying thread pools.

## Description

This talk will first present the notion of an execution context, then explore more deeply the types of thread pools that generally support them. It will feature an example that illustrates points of interest via a running application. By the end of the talk the audience will know what is happening under the hood when they use the Global Execution Context, as well as when to create multiple execution contexts.  Furthermore, they will be presented with a simple thread pool monitoring strategy and shown some configurations and usages that often lead to problems.  The idea for this talk is based on a real world production issue we encountered at Troops.ai.

## Notes

The talk will feature slides and live coding examples. As a Java veteran who made a transition to Scala a year ago -- I was fascinated at how familiar the underlying details of execution contexts were. While an opaque construct that “just works,” ECs are rife with opportunities to cripple your application. Many engineers coming to Scala use ECs without knowledge of their inner workings and will benefit from this deeper exploration.

## Bio
  
Scott is an early engineer at Troops who came to functional programing from the Java world. Previously he has worked for Cortica, a computer vision startup, and Ask.com