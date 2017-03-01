#The Hipster Stack

[Justin Bailey (m4dc4p)](http://twitter.com/m4dc4p)

[http://codeslower.com](http://codeslower.com)

Tozny, LLC

## Abstract

At Tozny, we're finding success using something we call "the hipster stack": http4s, doobie, OpenAPI and flyway. It's not LAMP and it's not MEAN, but it's working for us.


## Description

This talk explores how we put all the tools mentioned to use at Tozny while building E3DB, our end-to-end encrypted data store:

* Implementing REST APIs using http4s -- Combining the power of pattern-matching and extractors, plus the Task interface, makes implementing HTTP endpoints simple and fast.
* Database access using doobie -- No need for an ORM or complicated object model. Doobie gives us safe parameter interpolation and access to the full SQL language. Support for SQL dialects (e.g., mysql vs. Postgres) makes it easy to access vendor extensions.
* OpenAPI -- An OpenAPI specification lets us design and document our API before we write any code.
* Flyway -- Flyway lets us keep schema updates in the same repo as our code, and even migrates our databases for us automatically on deployment. Paradise!

I'll discuss the challenges and success we've had with all these tools.

(Why "The Hipster Stack"? Because all the cool kids are using it, of course!)

## Notes

This talk is more of an "experience report." I'll share how we are using these tools in production, and how I think they've accelerated development of our product. 

## Bio
  
I started my professional career as a object-oriented fundamentalist, but got blindsided by functional languages when I went back to graduate school. Scala has helped me combine those two disciplines into one.

I am also the author of the Haskell Cheatsheet (http://cheatsheet.codeslower.com), and maintain the HaskellDB library (http://github.com/m4dcc4p/haskelldb). 