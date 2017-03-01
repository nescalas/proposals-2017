#Guard against traffic oversaturation in the age of microservices

[Kai(luo) Wang (kailuowang)](http://twitter.com/kailuowang)

[http://kailuowang.github.io](http://kailuowang.github.io)

iHeartRadio Inc.

## Abstract

Traffic oversaturation (incoming traffic exceeding capacity), is prone to happen in complex microservice systems. They could quickly degrade the system with high latency and heavy memory usage. Let's talk about several strategies that can be used to exert backpressure during traffic oversaturation. 

## Description

When traffic oversaturation occurs, all the excessive traffic will have to wait in some queues in the service. The latencies grow exponentially to the point where no requests get served within the acceptable time frame. Worse, if the incoming traffic doesn't significantly slow down due to the high latency, e.g. when the users keep retrying regardless of the failed requests, the service will likely to experience an out-of-memory melt-down further down the line.

There are two types of traffic oversaturation scenarios which I will call as *positive oversaturation* and *negative oversaturation* respectively.
*Positive oversaturation* refers to the ones that occur when the incoming traffic increases to above the capacity;  *negative oversaturation* refers to the ones that occur when the capacity is so negatively affected that it's below the incoming traffic. Negative oversaturation happens more often in complex systems, such as microservice systems, where serving a request involves multiple layers of internal microservices and/or external dependencies. To name a few, network anomaly, external service degradation and disruptive competition of internal resources all can negatively affect the capacity of your service.

We'll talk about several strategies to deal with traffic oversaturation, namely 1) backpressure with a fixed throttle, 2) pull-based backpressure and 3) backpressure with an adaptive throttle. We'll also look into some traffic control schemes to work with these backpressure strategies. Finally, we will examine a Scala library that implemented the 3rd strategy. 




## Notes

Roughly 1.5 years ago I started with this question: how to guard our databases against DDOS attack? We then developed a library called [Kanaloa](http://github.com/iheartradio/kanaloa) for that purpose and deployed in our microservice system. In the process of developing this library, I learned a lot about traffic model and backpressure and the need of them in a microservice environment. This talk is oriented towards developers who are developing services but not quite familiar with those concepts. 

## Bio
  
Kai is a Scala developer who is passionate about open source software. He helps maintaining [typelevel/cats](http://github.com/typelevel/cats), [iHeartRadio/play-swagger](http://github.com/iHeartRadio/play-swagger), [milessabin/kittens](http://github.com/milessabin/kittens), [iHeartRadio/kanaloa](http://github.com/iHeartRadio/kanaloa), and [iHeartRadio/ficus](http://github.com/iHeartRadio/ficus).
Other things that interest him include photography, games, philosophy, travel and music composed by J.S. Bach. 