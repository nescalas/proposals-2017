#Reactive Kinesis Streams: An asynchronous Scala library for Amazon’s Kinesis

[Justin Potter & Mark Harrison (_j_potts)](http://twitter.com/_j_potts)

Weight Watchers International

## Abstract

Kinesis is Amazon’s answer to Kafka. After an overview of Kinesis and how we use it at Weight Watchers, we’ll discuss our open source library built using Scala & Akka to support Kinesis Streams. We'll cover the implementation details and explain how to use it, including error handling scenarios.

## Description

Architecting back-end services that meet the needs of a modern business is a challenging feat. Often, an engineer might turn to a “Reactive” micro-service based solution. Whilst this solves a lot of typical enterprise problems, it introduces a whole bunch of new ones! Developers will quickly run into issues once business analytics requirements and tight coupling between API’s begin rearing their ugly heads. Fortunately, we now have a number of choices available to solve this problem! 

This presentation will focus on Amazon’s Kinesis Streaming platform. Firstly why we chose this over the alternatives, followed by a discussion of the problems it solves. We’ll cover the decoupling of services, intra-service communication and analytics.

Next we’ll cover our open source Scala Kinesis library, built upon Akka. We’ll discuss why we decided to create a new library rather than simply using Amazon’s Java drivers. After an overview of the Kinesis architecture, we’ll dive into the design of the library and discuss the implementation patterns in detail - explaining our design choices for features such as async message processing, checkpointing, and handling of failures.

Finally we’ll explain how to take advantage of this new library, walking through configuration, code and error handling. We’ll cover various scenarios that must be considered, such as minimizing and dealing with message duplication.

Attendees will gain an understanding of Amazon Kinesis and why one would choose this solution. They’ll be ready to immediately start developing a Kinesis backed service, applying the techniques discussed in this talk to get a head start in their development.

## Notes

The talk will not expect attendees to have prior knowledge of Kinesis or it’s usage patterns. Enough background will be given to understand the use cases and the problems both Kinesis and in turn the library solve.

## Bio
  
**Justin Potter** is a passionate Scala developer and distributed systems engineer working at Weight Watchers International.  He is currently working on the Core Services team developing their new Reactive event-driven architecture.

**Mark Harrison** is a senior consultant for Cake Solutions, based in Manhattan. Currently he is working on the Core Services team at Weight Watchers International where he is helping to develop their new reactive architecture. He has over 10 years commercial experience and has been developing reactive and distributed applications using the Lightbend stack for over 5 years. Mark is also a Datastax certified Cassandra architect.