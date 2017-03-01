#Protobuf all the things

[Dan Billings (parqit)](http://twitter.com/parqit)

## Abstract

Forget HTTP and JSON and zoom straight to polyglot productivity by having protobuf/grpc types/plumbing generated for us.

## Description

Q. I suppose I should declare a JSON API?  Seems everybody uses it.  
A.  [Protobuf](https://developers.google.com/protocol-buffers/) offers types and is easily serialized/deserialized.  It is easy to declare, fast to use (parsers are generated for you), and safer to use (JSON parser code is a common source of bugs).

Q. I'm new to scala.  Which HTTP client/server should I use?  
A. [Grpc](http://www.grpc.io/) will **generate server and client glue** and has some nice security features too.  

**Forget about these boondoggles** and focus on adding value.  Write a service that can be consumed using absolute minimal boilerplate by a wide array of languages.

We'll see how easy it is to:  
 * define a structured API and implement it.  [ScalaPB](https://scalapb.github.io/) will generate some tasty Scala for our use.   
 * consume a grpc API by playing w/ [Google's speech](https://cloud.google.com/speech/) [API](https://github.com/googleapis/googleapis/blob/master/google/cloud/speech/v1beta1/cloud_speech.proto) .  

## Notes

I see lots of bugs introduced in highly boring places such as JSON parsers and HTTP frameworks.

This is my attempt to be the change I want to see in the world.

## Bio
  
I've written Scala for 2 startups and a Fortune 15 company and thus have seen a lot of sausage made.  I've got good ideas to get past common rough spots and more readily focus on core competencies.

