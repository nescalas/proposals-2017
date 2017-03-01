#Validating Domain Objects with Cats

[Mike Gehard (mikegehard)](http://twitter.com/mikegehard)

Wunder Capital

## Abstract

One common problem in any application is the validation of user input. This talk will outline one approach using the Validated data type from the Cats library. Attendees will come away with an understanding of how to use the library via a simple demonstration.

## Description

The life of a developer would be much easier if we didn't have to deal with pesky users trying to break out software at every turn. In order to keep the hordes from breaking down the gates of our pristine software castles, implementing validations for user entered data is of the utmost importance.

In this talk, attendees will see one way to implement a functional validation layer using the Validated data type from the Cats library. Along the way we will talk about what goes into a good validation library, the mistakes we made when writing our code and even throw in some functional patterns from the Cats library.


## Notes

As someone who is a relative newcomer to the Scala landscape, I feel like I have a good connection with beginners who are just coming to the Scala landscape. My long running career in software (~15 years) allows me to bring analogies from other languages to bear with talking with folks.

Also, I've just finished writing our validation layer in a new app so I can talk about all of the pitfalls that more seasoned Scala developers may have forgotten about.

## Bio
  
Mike is the VP of Engineering at Wunder Capital, a small startup that provides commercial solar financing. Before Wunder, he dabbled in Scala but is now the lead developer on a new application written in Scala. This "beginner's mind" allows him to speak to the masses who want to understand the functional power of Scala but still think that a monad is a burrito or have heard about applicative functors but have no idea how to use them.