#Azure cloud storage client optimization with PlayFramework and Scala 

Arkady Bari

[https://www.linkedin.com/in/arkady-bari-75279a3](https://www.linkedin.com/in/arkady-bari-75279a3)

Comcast Corporation

## Abstract

Comcast Continuous Video Recording (CVR) Service must handle concurrent video uploads to Azure Cloud from hundreds of thousands of cameras. The presentation will go over details on how we optimized our service performance leveraging asynchronous nature of PlayFramework and SCALA concurrency support.

## Description

Azure provides Java Client to perform basic CRUD operations against cloud storage. While very easy to use, it does not perform well under load; it causes thread contention and suboptimal performance. In lieu of Azure Java Client we have chosen non-blocking http client built in into Play Framework to make Azure Storage Restful API requests. This allowed us to greatly improve performance by decoupling the number of threads from the number of concurrent requests. We also implemented non blocking retries utilizing Akka Schedulers and Scala Promises. I will go over the details of the implementation.  

## Notes

The task to support video uploads from hundreds of thousands of cameras was daunting. Our Service handles over 7 thousands requests per second, uploads 2000 hours worth of videos every minute, extracting  50 million images per day. Apart from setting up massive infrastructure to support this we made concerted efforts to optimize our code. I was a principal implementor of this solution and would like to share my experience

## Bio
  
I am a seasoned software engineer having many years of experience building and designing distributed high performance for Home Security/Automation systems utilizing open source solutions such as Kafka, Twitter Storm, Cassandra.