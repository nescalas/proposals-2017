#giphykube

[Randy Shepherd & Sean Carey (aut0mat0n1c)](http://twitter.com/aut0mat0n1c)

Giphy

## Abstract

Scala is a leading choice for building microservices. However, tools like ConductR are useful if you have a pure Scala ecosystem. How is service orchestration done in a polyglot environment? How can one write and test code for these systems without pain?  'giphykube' solves both these problems.

## Description

Microservices are a dominant architectural model in modern software engineering. The benefits are understood but so are the trade-offs, some of which are operational in nature. 

Scala is a leading choice for building microservices. However, tools like ConductR are useful if you are running a completely Scala ecosystem. How is service orchestration done in a polyglot environment? And in such an environment, how can a developer write and test code for these systems without pain? 

At Giphy we have developed a tool we call 'giphykube' that solves for both these problems. One of the driving reasons for development of ‘giphykube’ was to hide the delivery-oriented mechanisms of Kubernetes and containers, allowing application developers to focus on developing applications. In its current form, ‘giphykube’ encapsulates all runtime dependencies (Scala, Jvm, Python, databases, monitoring, etc) within the container image, while dynamically passing application code into the running container in the cloud as it is edited locally by the developer in a completely transparent manner. Note that this cloud-based container is a pared down production environment replicant. Therefore all system dependencies are present enabling integration testing of new code in seconds.

We plan to open source this project and would look forward to giving a sneak peek.

## Notes

Who would actually give this talk is a little up in the air, we were considering doing it as a pair.. somebody representing eng and somebody representing devops. That is the nature of the tool and seems like a good strategy. 

## Bio
  
Randy Shepherd VP of Eng @ Giphy & Sean Carey Director of DevOps @ Giphy