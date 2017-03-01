#Scala REPL for Scio/Apache Beam

[Rafal Wojdyla (ravwojdyla)](http://twitter.com/ravwojdyla)

Spotify

## Abstract

Scio is a Scala API for Apache Beam inspired by Spark and Scalding. Scio not only adds Scala API, but also number of extra features to Apache Beam. One of them is Scala REPL, which allows for rapid prototyping of your data pipeline. From this talk you will learn exactly why and how we have built it.

## Description

[Scio](https://github.com/spotify/scio) is a Scala API for [Apache Beam](https://beam.apache.org/) inspired by [Spark](http://spark.apache.org/) and [Scalding](https://github.com/twitter/scalding). It puts a civilized and familiar functional DSL on top of Apache Beam, but that is not all, it also comes with number of extra features while keeping all the goodies of Apache Beam. One of the extra features is Scala REPL (Read-Eval-Print Loop), which allows for rapid prototyping and testing of your data pipeline.

From this talk you will learn, why and how we have built it. We will walk through the problem, limitations, ideas we have tried (and failed), as well as current working solution. We will touch upon Serialization mechanisms, original Scala REPL, Classloaders, distributed processing and well as Apache Beam execution internals.

## Notes

Hello,
This would be rather advanced topic, and will touch upon multiple interesting problems, specifically around distributed data processing and Scala. I'm the author of Scio REPL, and one of the developers of Scio which gives me an unique perspective to share my knowledge about this problem. Previously I gave a couple of talks including, but not limited to: Strata + Hadoop World San Jose 2015, Hadoop Summit Brussels 2015 and GOTO Conferences and number of meetups.
Cheers - Rafal

## Bio
  
Rafal has been working with data storage and processing for more than 6 years, more recently at Spotify. First as part of team that has built the Hadoop clusters from 1 node to more than 2 thousands nodes in the span of last 3 years. Now as part of team working with data processing libraries. Rafal is a contributor to [Scio]((https://github.com/spotify/scio) (Scala API for Apache Beam), [snakebite](https://github.com/spotify/snakebite) (pure python HDFS client), author of [gcs-tools](https://github.com/spotify/gcs-tools) and more.