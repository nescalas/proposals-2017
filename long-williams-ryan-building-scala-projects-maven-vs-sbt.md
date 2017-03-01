# Building Scala Projects: Maven vs. SBT

[Ryan Williams (runsascoded)](https://twitter.com/RunsAsCoded)

[https://www.linkedin.com/in/ryan-williams-44a4212/](https://www.linkedin.com/in/ryan-williams-44a4212/)

Hammer Lab at Mount Sinai School of Medicine

## Abstract
Is there a way to cross-publish libraries for multiple Scala binary versions in Maven without using `sed` to rewrite POMs? I recently tried and failed in about a dozen ways before porting my universe to SBT.

Come for a discussion of specific Scala build-processes, stay for reflections about workflows, eDSLs, and build configuration in general!

## Description
A complete encapsulation failure can be found at the heart of the build-/release-processes of a dozen of the most prominent open-source Scala projects.

It has several names, most commonly [`change-scala-version.sh`](https://github.com/apache/spark/blob/v2.1.0/dev/change-scala-version.sh), and it combs a regular-expression over `pom.xml` files, changing `2.11`s to `2.10`s (or vice versa), in order to cross-publish libraries for both Scala binary-versions.

This is the wrong place to solve this problem by about 4 layers of abstraction. How did this happen? Can we do better?

In this talk I'll outline some failed attempts to make Maven play nice with Scala-ecosystem idiosyncracies. I'll also discuss broader epiphanies about why Scala projects should not shoehorn build- and release-management into logic-less XML configs consumed by Java(-bean)-based plugins, but rather should expect to bring all of the power and sophistication of Scala to bear on their project-management that they do on their projects' source.

## Notes
I've written in Scala for about 6 years, and built projects with SBT, Maven, and Pants for about 2 years each.

Build-tool comparisons notoriously-easily degenerate into bikeshed-Sarlaac-pits, but I will try to give an even-handed account of each tool here, based on my experience as well as some first-principles derivation of what we might ask of them in a more perfect world.

## Bio
I'm a software developer at [Hammer Lab](http://www.hammerlab.org/) at Mount Sinai School of Medicine, where I write distributed genomic-analysis tools in Scala that run on Apache Spark.

Previously, I worked on various web-servers in Scala at Foursquare.