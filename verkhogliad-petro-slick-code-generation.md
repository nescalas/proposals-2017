#Slick code generation

[Petro Verkhogliad (vpetro)](http://twitter.com/vpetro)

[]()

Lightbend

## Abstract

sbt-slick-codegen is an sbt plugin that with a few lines of configuration
removes the pain of writing out Slick database schema when
working with or evolving an existing database schema.


## Description

slick-codegen-plugin is an sbt plugin that with a few lines of configuration
removes the pain of writing out Slick database schema when
working with or evolving an existing database schema.

In this session we will discuss and demo an sbt plugin for schema generation
with Slick (http://slick.lightbend.com) that with a few lines of configuration enables:

  - generation of tagged id types for primary and foreign keys 
  - restricting schema generation to specific tables
  - separation of row and table specifications into distinct compilation units
  - customizable mappings between application and database types

During the demo we will setup and use the plugin in a sample project.

## Notes

This talk will be delivered by the two co-authors of the plugin: Stewart Stewart and Petro Verkhogliad. This work arises from real-world experience of working with Slick and legacy database schemas. The feelings of safety of having a database schema described in Scala are sometimes dwarfed by the pain of actually having to write and maintain the Scala mappings. This becomes obvious when building a new project with an existing database.

The code generation component is bundled with Slick. However, the documentation shows only the most trivial use-case. With every new project we have updated and expanded on the use-cases the plugin covers. Now, we would like to share what we have built and learned.

Stewart Stewart is a Scala software engineer at Driver Group, conference speaker and Scala meetup co/organizer in San Francisco and New York.
Petro Verkhogliad is a Scala consultant/trainer at Lightbend and Scala meetup organizer in Ottawa, Canada.

## Bio
  
Petro Verkhogliad is a senior consultant and trainer at Lightbend. Previously a university instructor, Petro is passionate about Scala, functional programming and applications of AI.