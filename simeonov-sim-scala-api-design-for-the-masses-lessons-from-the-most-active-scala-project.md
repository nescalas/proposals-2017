#Scala API design for the masses: lessons from the most active Scala project

[Sim Simeonov (simeons)](http://twitter.com/simeons)

[http://linkedin.com/in/simeons](http://linkedin.com/in/simeons)

Swoop, Inc.

## Abstract

Apache Spark, a fast and general engine for big data processing, has quickly overtaken Akka to become the most popular and most active open-source project in Scala. This talk explores how Spark uses Scala internally and dives deep into Spark's external API design choices.

## Description

Chances are you that you haven't used [Apache Spark](http://spark.apache.org/). This is your chance to learn about and learn from the most active open-source Scala project.

Spark is unique in many ways. It didn't grow out of the Scala community the way major Scala projects did. It came out of UC Berkeley. Scala was chosen almost by accident for one key feature (serializable closures) yet the choice of Scala fundamentally influenced Spark's core. Spark wasn't trying to replicate existing approaches in Scala the way Akka drew from Erlang and Play from Ruby on Rails. It introduced a fundamentally new way of working with big data. It remains unique for its approach and it's taking the world by storm.

Programming language communities are shaped by their most popular frameworks and the problems these frameworks are tackling: Java by J2EE, Scala by Akka & Play, Ruby by Rails, etc. If you care about the evolution of the Scala community, you should be very interested in how Apache Spark, the new gateway drug pulling developers into Scala, is using the language.

Framework and API design patterns are hugely influenced by three factors: codebase size, number of contributors and target developer profiles. If you are are interested in what it takes to create super-popular large Scala projects with many contributors and hundreds of thousands of users, you should be very interested in how Apache Spark, which has 3x the codebase size and 3x the number of contributors of Akka, is succeeding & failing at API design.

Last but not least, if you like to solve hard problems at scale, you should be very interested in Apache Spark both as a place to contribute to open-source and because Spark-related work is quickly becoming the fastest growing segment of Scala job opportunities in the US.

## Notes

In my conversations with Scala enthusiasts I'm continually surprised by their lack of awareness about Apache Spark. Looking at open-source metrics as well as developer + enterprise adoption trends and job postings, Spark is not only the most active Scala project in the world but also the force behind the largest net-new increase in Scala job opportunities, at least in the US. For those reasons alone, it would be helpful to spread awareness about Spark in the Scala community.

There is an even better reason to mix the Spark community and the Scala community. It involves learning and sharing best practices about large codebase management and API design for mass usage. There is a sub-trend in the Scala community to create beautiful but inaccessible frameworks and this hurts Scala's mass adoption. Spark has made some interesting--one might argue controversial--choices in its use of Scala. I'd like to review Spark's opinionated design choices in the talk with examples of cases where they work very well, as witnessed by Spark's adoption by hundreds of thousands of developers, and where they fail, e.g, where simplicity comes at the expense of making framework-level extensions by third parties extremely difficult.

I'd like to do this talk in part because I bring a unique perspective informed by pattern recognition from lots of scar tissue. I am a relative newcomer to the Scala community but my background is in programming language, framework and API design. My first startup invented the mixing of code and HTML in templates back in 1994. I was the chief architect of the first Web application server--ColdFusion--used by 500+ thousand developers. Thousands of partners built frameworks and products on top of ColdFusion. Later, I was chief architect at Macromedia, working across platform products used daily by 2.5 million developers and designers. I've done lots of open-source work with the Apache Foundation (my team at Macromedia and some IBMers built the most popular Web services engine), the Java Community Process (messaging and a few other standards) and the W3C (SOAP).

I have deep roots in the Apache Spark community. While I'm too busy with Swoop to contribute directly to Spark, I have close relationships and regular conversations with its architects and occasionally open-source some of our Scala stack (e.g., [spark-records](https://swoop-inc.github.io/spark-records/)). I speak frequently at the Spark Summit and am one of the judges of talk submissions. 

If you want to see what I'm like speaking, [here is an example](https://spark-summit.org/2016/events/bulletproof-jobs-patterns-for-large-scale-spark-processing/).

If you want to talk to someone from the Scala community who knows me, Nermin would be the best choice.

Thanks for the consideration!

## Bio
  
[Simeon Simeonov](http://linkedin.com/in/simeons) likes to solve big, hard problems with small, easy-going teams. He is the founder & CTO of Swoop where he is tackling petabyte-scale big data and machine learning problems using Apache Spark and Scala. In a prior life, Sim built compilers and interpreters used by hundreds of thousands of developers and was the chief architect of the first Web application server (ColdFusion) and one of the largest platform companies in the US (Macromedia, now Adobe). He's contributed to popular APIs and standards through the Apache Foundation, the Java Community Process and the W3C. Sim blogs at blog.simeonov.com, tweets as @simeons and lives in the Greater Boston area with his wife, son and an adopted dog named Tye.