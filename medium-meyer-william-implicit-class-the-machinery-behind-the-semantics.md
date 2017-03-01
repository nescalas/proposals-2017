#Implicit Class - The Machinery Behind the Semantics

[William Meyer (williammmeyer)](http://twitter.com/williammmeyer)

Troops.AI

## Abstract

In this talk, I'll trace a simple program through the Scala compiler explaining the phases and data structures used to parse and de-sugar source code, infer types, lookup methods and apply implicit conversions.

## Description

Many Java APIs are unwieldy or unsafe but Scala gives us the tools to improve them - implicit classes are a great way to reduce boilerplate and increase expressiveness in our code.

In this talk, I’ll discuss implicit views in the Scala Language Specification and implicit classes in Scala Improvement Proposal-13 and present a simple program that uses implicit classes to wrap an unsafe API. Then we’ll trace the compilation of the program through scalac.

I’ll present the major data-structures (Compilation Unit, Context, Tree, Symbol & Scope) and phases (parser, namer & typer) in the compiler and then we’ll dive into the code and learn how scalac represents, transforms, and types our simple program.

## Notes



## Bio
  
Will was the first engineer at Troops.AI and a functional programing veteran. He graduated from NYU with a degree in math and econ and then spent 3 years at Novus Partners as both individual contributor and a team lead.