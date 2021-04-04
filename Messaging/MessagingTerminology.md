
# Messaging Terminology

This document was started to proivde  handy reference citation for getting alignment within teams and organizations on
the definition of various terms that are often used when discussing messaging, event driven architecture, and real-time data streaming.   


- Terms of Art (_"a word or phrase that has a precise, specialized meaning within a particular field or profession."_)
  + Messaging:
    * Message
    * Message Broker
    * Messaging Framework
    * Message Oriented Middleware (MOM)

  + Streaming
    * Event
    * Streaming Platform
    * Event Stream Platform

  + Pub/Sub

- Useful distinction..._?_
  + real-time data streams 
  + messaging



## Solution Citations/References

## Kafka 
- https://www.confluent.io/blog/event-streaming-platform-1/
  + *Putting Apache Kafka To Use: A Practical Guide to Building an Event Streaming Platform (Part 1, 2015)*

  + _"applications that triggered asynchronously off of activity elsewhere in the system"_
  + _"core work decoupled from the UI actions that triggered them"_
  + _"Our messaging systems were low latency but unreliable and unscalable."_
  + _"We needed something asynchronous from the user but fast."_
  + _"we mostly ended up trying to cram these requirements into databases and request response services that were a particularly unnatural fit."_

  + _"As originally imagined"_, source:confluent.io
    * ![](https://cdn.confluent.io/wp-content/uploads/streaming-platform-2-768x802.png)

  + _"A modern stream-centric data architecture built around Apache Kafka"_, source: confluent.io
    * ![](https://cdn.confluent.io/wp-content/uploads/data-flow-768x584.png)

  * _"a kind of universal pipeline for data"_
    * _"Continuous feeds of well-formed data act as a kind of lingua franca across systems, applications, and data
      centers."_

  + _"Today at LinkedIn Kafka handles over 1 trillion events per day spread over a number of data centers"_

  + _"Most of what a business does can be thought of as streams of events."_

  + _"Retail has streams of orders, sales, shipments, price adjustments, returns, and so on. Finance has orders, stock prices, and other financial time series. Web sites have streams of clicks, impressions, searches, and so on. Big software systems have streams of requests, security, errors, machine metrics, and logs. Indeed one view of a business is as a kind of data processing system that takes various input streams and produces corresponding output streams (and maybe some physical goods along the way)._

  + _*"This view of data can seem a little foreign to people who are more accustomed to thinking of data as rows in
    databases rather than as events"*_

  + _"An event streaming platform has two primary uses:"_
    * _"Stream processing: It enables continuous, real-time applications built to react to, process, or transform
      streams. This is the natural evolution of the world of Enterprise Messaging which focused on single message
      delivery, stream processing gives you that and more."_
    * _"Data Integration: The event streaming platform captures streams of events or data changes and feeds these to
      other data systems such as relational databases, key-value stores, Hadoop, or the data warehouse. This is a
      streaming version of existing data movement technologies such as ETL systems."_

  + _"key capabilities of an event streaming platform:"_
    * _"Pub/Sub: An event streaming platform must enable real-time publishing and subscribing to data streams at
      scale..."_
    * _"Process: It must enable the real-time stream processing of streams at scale "_
    * _"Store: It must be able to reliably store streams of data at scale. "_

  + _*"Apache Kafka is a distributed system designed for streams"*_

  + _*"Kafka is often categorized as a messaging system, and it serves a similar role, but provides a fundamentally different abstraction. The key abstraction in Kafka is a structured commit log of updates"*_
    * source: confluent.io
      * ![](https://cdn.confluent.io/wp-content/uploads/2016/08/commit_log-copy.png)

  + _"An event streaming platform is similar to an enterprise messaging system—it receives messages and distributes them to interested subscribers. "_
    * "There are three important differences:"
      * "Messaging systems are typically run in one-off deployments for different applications"
      * "Messaging systems do a poor job of storing data and this limits them to streams which have only real-time consumption"
      * "Messaging systems do not provide semantics that are easily compatible with rich stream processing"

  + _"an event streaming platform is a messaging system whose role has been re-thought at a company-wide scale."_


## Background Reading

- https://stackoverflow.com/questions/41744506/difference-between-stream-processing-and-message-processing
  +
    * Messaging is communication between two or more processes (or components) 
    * Streaming is the passing of event log activities - as they occur. 

  + 
    * Messaging carries raw data
    * Events contain information about an occurence/activity. 

  + 
    * Traditional messaging systems cannot go "back in time" (i.e., messages are deleted from a queue once they delivered
    to all subscribing consumers
    * Streaming processing (i.e., as supported by Kafka) supports more complex applications - e.g., keeping messages (for a configurable period of time) - allowing consumers to "rewind" and consume messages
    multiple times - or if a new consumer is added, they can read the complete history. 
      * Kafka offers Kafka Connect and Streams API - so it supports stream processing - as well as messaging/pub-sub

  + 
    * Micro-batching encompasses the idea of a boundary window - and has an implication of when to execute.
    *  A stream (generally) could be considered a micro-batch, with a window size of [1] - and processes the
    record/event/fact as it arrived.

  + 
    * A stream might be infinite
    * Batch processing may be considered as a special case of stream processing (with a strongly defined window)

  + 
    * Message processing implies operations on individual messages.
    * Stream processing may imply operations on individual messages - as well as operations on collection of messages - as
    they flow into a system.


