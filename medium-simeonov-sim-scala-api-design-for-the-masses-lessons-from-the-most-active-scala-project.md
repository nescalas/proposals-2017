#Scala API design for the masses: lessons from the most active Scala project

[Sim Simeonov (simeons)](http://twitter.com/simeons)

[http://linkedin.com/in/simeons](http://linkedin.com/in/simeons)

[Swoop, Inc.](http://www.swoop.com)

## Abstract

Apache Spark, a fast and general engine for big data processing, has quickly overtaken Akka to become the most popular and most active open-source project in Scala. This talk explores how Spark uses Scala internally and dives deep into Spark's external API design choices.

## Description

Chances are you that you haven't used [Apache Spark](http://spark.apache.org/). This is your chance to learn about and learn from the most active open-source Scala project.

Spark is unique in many ways. It didn't grow out of the Scala community the way major Scala projects did. It came out of UC Berkeley. Scala was chosen almost by accident for one key feature (serializable closures) yet the choice of Scala fundamentally influenced Spark's core. Spark wasn't trying to replicate existing approaches in Scala the way Akka drew from Erlang and Play from Ruby on Rails. It introduced a fundamentally new way of working with big data. It remains unique for its approach and it's taking the world by storm.

Programming language communities are shaped by their most popular frameworks and the problems these frameworks are tackling: Java by J2EE, Scala by Akka & Play, Ruby by Rails, etc. If you care about the evolution of the Scala community, you should be very interested in how Apache Spark, the new gateway drug pulling developers into Scala, is using the language.

Framework and API design patterns are hugely influenced by three factors: codebase size, number of contributors and target developer profiles. If you are interested in what it takes to create super-popular large Scala projects with many contributors and hundreds of thousands of users, you should be very interested in how Apache Spark, which has 3x the codebase size and 3x the number of contributors of Akka, is succeeding & failing at API design.

Last but not least, if you like to solve hard problems at scale, you should be very interested in Apache Spark both as a place to contribute to open-source and because Spark-related work is quickly becoming the fastest growing segment of Scala job opportunities in the US.

## Bio
  
[Simeon Simeonov](http://linkedin.com/in/simeons) likes to solve big, hard problems with small, easy-going teams. He is the founder & CTO of Swoop where he is tackling petabyte-scale big data and machine learning problems using Apache Spark and Scala. In a prior life, Sim built compilers and interpreters used by hundreds of thousands of developers and was the chief architect of the first Web application server (ColdFusion) and one of the largest platform companies in the US (Macromedia, now Adobe). He's contributed to popular APIs and standards through the Apache Foundation, the Java Community Process and the W3C. Sim blogs at [blog.simeonov.com](http://blog.simeonov.com), tweets as [@simeons](http://twitter.com/simeons) and lives in the Greater Boston area with his wife, son and an adopted dog named Tye.
