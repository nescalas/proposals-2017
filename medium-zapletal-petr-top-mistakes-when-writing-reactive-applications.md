#Top Mistakes When Writing Reactive Applications

[Petr Zapletal (petr_zapletal)](http://twitter.com/petr_zapletal)

[https://www.linkedin.com/in/petr-zapletal-5409654a](https://www.linkedin.com/in/petr-zapletal-5409654a)

Cake Solutions

## Abstract

Reactive applications are becoming a de-facto industry standard. But design of these systems might be challenging as it requires particular mindset shift to tackle problems we might not be used to. We’re going to discuss things I’ve seen in the field that prevented applications to work as expected.


## Description

Reactive applications are becoming a de-facto industry standard and, if employed correctly, toolkits like Lightbend Reactive Platform make the implementation easier than ever. But the design of these systems might be challenging as it requires particular mindset shift to tackle problems we might not be used to. In this talk, we’re going to discuss the most common things I’ve seen in the field that prevented applications to work as expected. I’d like to talk about typical pitfalls that might cause troubles, about trade-offs that might not be fully understood or important choices that might be overlooked including persistent actors pitfalls, tackling of network partitions, proper implementations of graceful shutdown or distributed transactions, trade-offs of micro-services or actors and more. 

This talk should be interesting for anyone who is thinking about, implementing, or have already deployed a reactive application. My goal is to provide is to provide a comprehensive explanation of common problems to be sure they won’t be repeated by fellow developers. The talk is a little bit more focused on Lightbend platform but understanding of the concepts we are going to talk about should be beneficial for everyone interested in this field.

## Notes

Spoke in NE Scala last year and would be honored if I could speak there again.

## Bio
  
Petr is a Consultant who specializes in the design and implementation of highly scalable, reactive and resilient distributed systems. He is a functional programming and open source enthusiast and has expertise in the area of big data and machine classification techniques.

Petr participates in the whole software delivery life-cycle: from requirement analysis & design through to maintaining systems in production. During his career, Petr has worked for various companies, from start-ups to large international corporations.

Technically, Petr is SMACK (Spark, Mesos, Akka, Cassandra, Kafka) evangelist. Petr enjoys working with Akka and has deep knowledge of toolkit’s features like Akka Clustering, Distributed Data or Akka Persistence. Petr is also certified Spark Developer.

Petr has extensive speaking experience mostly from various meetups or corporate training/presentations but also from larger conferences like Scala.exchange, ScalaDays, Scala by the Bay, Spark Summit or last NE Scala