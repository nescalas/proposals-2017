#Protocol Independent APIs : Make your API Web and CLI accessible 

[Kishore Reddy (kishore_reddy)](http://twitter.com/kishore_reddy)

[http://www.codehelix.co](http://www.codehelix.co)

CodeHelix Solutions

## Abstract

API design patterns with an emphasis on building Protocol Independent APIs. 
This involves writing your API once and hosting the API as a Web API ( via Akka-Http ), using it on a CLI (command line interface), or in a batch process for automation purposes. 

## Description

API design patterns with an emphasis on building Protocol Independent APIs. 
This involves writing your API 1 time and hosting the API as a Web API ( via Akka-Http ), using it on a CLI (command line interface), or in a batch process for automation purposes. Various concepts/approaches/techniques will be mentioned that can yield APIs to not just solve business problems but also provide significant value to QA/Test engineers, DevOps, and even Support Teams.

# Overview
- Inform audience on various trends in API design and implementation
- Inform audience on some tools and frameworks available ( Google GRPC, Twitters Finagle, Facebooks Graph QL, Swagger )
- Inform audience on general industry trend towards making APIs more accessible, discoverable, and simpler ( via removing protocol code and noise )
- Inform audience on small to moderate techniques to achieve API accessibility, discoverability and  easy of development 
- Inform audience on designing APIs in ways that can add significant value to QA/Test engineers, DevOps, and even Support Teams
- Demo the techniques using a small example of an API in Scala that can be run as Web API and also available on the CLI ( command line )

# Sections
- **API Routing**        : A simple unified routing format for both Web/Http and CLI
- **API Container**    : How to wrap your APIs inside of a container
- **API Registration** : How to register your APIs and make them available 
- **API Discovery**    : How to make your APIs discoverable 
- **API Hosting**      : Running your APIs via Akka-Http or a CLI

NOTES:
Will demo writing your API in Scala as a plain class and various approaches to making it available as both a Web API ( using Akka-Http ) and on the CLI ( command line interface ) shell.

TECH: 
While the concept is language independent, it will include a working example using: 
1. Scala
2. Akka-Http
3. Command Line Interface

## Notes

I've presented this topic at the Code Camp NYC 2017 available here http://codecampnyc.org/schedule/ but on a slighter more smaller scale.  Just select option to show all the items and search for "Kishore Reddy". While I've worked in a team-lead, architect, and full-stack roles, my main area of expertise has always been API design and that has lead to me develop both private and public ( open-source ) solutions building APIs that are scalable, testable, and versatile. I'm uniquely interested in the area where an API can provide ways for multiple teams to inter-connect and access shared information in simple ways. 

I'm also currently developing an open-source Scala Tool Kit  called Slate Kit, available at www.slatekit.com. It is currently in a private beta, and not advertised until a future public release. This abstract/presentation uses concepts inspired from Google GRPC, Twitter's Finagle, and Swagger, and 1-2 concepts of my own, but does NOT use my open-source code, and is framework independent. 


## Bio
  
My name is Kishore Reddy and I'm a New York City based Software Architect, Entrepreneur, open-source and mobile app developer. Over the last 12-14 years, I've focused on building solutions for various industries. 


I'm also currently developing an open-source Scala Tool Kit  called Slate Kit, available at www.slatekit.com. It is currently in a private beta, and not advertised until a future public release. This abstract/presentation uses concepts inspired from Google GRPC, Twitter's Finagle, and Swagger, and 1-2 concepts of my own, but does NOT use my open-source code, and is framework independent. 


