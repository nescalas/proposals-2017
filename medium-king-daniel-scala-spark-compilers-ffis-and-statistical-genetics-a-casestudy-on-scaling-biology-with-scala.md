#Scala, Spark, Compilers, FFIs, and Statistical Genetics: A Case-Study on Scaling Biology with Scala

[Daniel King (danking00)](http://twitter.com/danking00)

[https://hail.is](https://hail.is)

Broad Institute

## Abstract

Hail is an open-source tool for scalable statistical genetics. We use compiler & language techniques for a domain-specific language; Spark to orchestrate the data and computation across cloud clusters; and the FFI for the jet engines. I'll explain how we put it together to analyze 40TB of genomes.

## Description

Hail is an open-source tool for statistical genetics built by a small team of software engineers embedded in a scientific lab.

In just a year-and-a-half, our team has built the leading tool for handling statistical genetics datasets in the 10s of TB. Our success was enabled by the high-level expressiveness and type-safety of Scala as well as the rich library ecosystem, most notably Spark. Along the way, we've enjoyed the pleasures of Scala, suffered the pains, and engineered around the holes. In this talk I'll give a brief overview of our problem domain before diving into the language and distributed-runtime-system that we've built on top of Scala and Spark. Our work includes a nascent library facilitating safe, concise generation of JVM byte code; ideas for handling multi-dimensional data on top of RDDs (including a custom RDD class to support datasets too large to be shuffled); and playing bit-fiddling tricks on the other side of the FFI.

I could probably build the talk for any of the proposed time lengths.

## Notes

The talk will only assume knowledge of Scala; however knowledge of Spark, FFIs & SIMD, and linear algebra will likely enable a deeper understanding of the relevant sections.

I'm best qualified to talk on this subject because I'm a software engineer at the Broad Institute, a non-profit biological research institution. At the Broad, a work full-time on Hail. I work closely with geneticists to build the software primitives that enable them to do reproducible science at the 10s of terabytes scale.

## Bio
  
I'm a grad school drop out trying to bring programming language techniques to the "real world". I'm especially excited to build languages and tools that raise the abstraction level from bits and data structures to scientific concepts.

I'm also excited about soccer, running, math, and equality in tech and elsewhere.