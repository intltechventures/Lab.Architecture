
# Messaging Terminology

- Terms of Art (_"a word or phrase that has a precise, specialized meaning within a particular field or profession."_)
  + Messaging:
    * Message
    * Message Broker
    * Messaging Framework
    * Message Orietned Middleware (MOM)

  + Streaming
    * Event
    * Streaming Platform
    * Event Stream Platform


- Useful distinction
  + real-time data streams 
  + messaging



## Solution Citation

## Kafka 
- https://www.confluent.io/blog/event-streaming-platform-1/
  + _"applications that triggered asynchronously off of activity elsewhere in the system"_
  + _"core work decoupled from the UI actions that triggered them"_
  + _"Our messaging systems were low latency but unreliable and unscalable."_
  + _"We needed something asynchronous from the user but fast."_
  + _"we mostly ended up trying to cram these requirements into databases and request response services that were a
    particularly unnatural fit."_
  ![](https://cdn.confluent.io/wp-content/uploads/streaming-platform-2-768x802.png)



## Background Reading

- https://stackoverflow.com/questions/41744506/difference-between-stream-processing-and-message-processing
  + Messaging is communication between two or more processes (or components) 
  + Streaming is the passing of event log activities - as they occur. 

  + Messaging carries raw data
  + Events contain information about an occurence/activity. 

  + Traditional messaging systems cannot go "back in time" (i.e., messages are deleted from a queue once they delivered
    to all subscribing consumers
  + Streaming processing (i.e., as supported by Kafka) supports more complex applications - e.g., keeping messages (for a configurable period of time) - allowing consumers to "rewind" and consume messages
    multiple times - or if a new consumer is added, they can read the complete history. 
    * Kafka offers Kafka Connect and Streams API - so it supports stream processing - as well as messaging/pub-sub

  + Micro-batching encompasses the idea of a boundary window - and has an implication of when to execute.
  + A stream (generally) could be considered a micro-batch, with a window size of [1] - and processes the
    record/event/fact as it arrived.

  + A stream might be infinite
  + Batch processing may be considered as a special case of stream processing (with a strongly defined window)

  + Message processing implies operations on individual messages.
  + Stream processing may imply operations on individual messages - as well as operations on collection of messages - as
    they flow into a system.


