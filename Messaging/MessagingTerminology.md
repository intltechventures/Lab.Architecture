
# Messaging Terminology

This document was started to proivde  handy reference citation for getting alignment within teams and organizations on
the definition of various terms that are often used when discussing messaging, event driven architecture, and real-time data streaming.   


- Terms of Art (_"a word or phrase that has a precise, specialized meaning within a particular field or profession."_)
  + Messaging:
    * Message

    * Message Passing
      * https://en.wikipedia.org/wiki/Message_passing


    * Queue
      * https://en.wikipedia.org/wiki/Queue_(abstract_data_type)

    * Message Queue 
      * https://en.wikipedia.org/wiki/Message_queue
        * _"In computer science, message queues and mailboxes are software-engineering components typically used for inter-process communication (IPC), or for inter-thread communication within the same process. They use a queue *for messaging – the passing of control or of content*."_

    * Message Broker

    * Messaging Framework

    * Message Oriented Middleware (MOM)
      * https://en.wikipedia.org/wiki/Message-oriented_middleware
        * "software or hardware infrastructure supporting sending and receiving messages between distributed systems"
        * "Using a MOM system, a client makes an API call to send a message _*to a destination managed by the provider*._ The call invokes provider services to route and deliver the message."
        * "MOM comprises a category of inter-application communication software that generally relies on asynchronous
          message-passing, as opposed to a request-response architecture. In asynchronous systems, message queues
          provide temporary storage when the destination program is busy or not connected. In addition, most
          asynchronous MOM systems provide persistent storage to back up the message queue."
        * "The primary disadvantage of many message-oriented middleware systems is that they require an extra component in the architecture, the message transfer agent (message broker)."


  + Streaming
    * Event

    * Stream Processing
      * https://en.wikipedia.org/wiki/Stream_processing
        * "Stream processing is a computer programming paradigm, equivalent to dataflow programming, event stream
          processing, and reactive programming..."
        * "The stream processing paradigm simplifies parallel software and hardware by restricting the parallel
          computation that can be performed. Given a sequence of data (a stream), a series of operations (kernel
          functions) is applied to each element in the stream. Kernel functions are usually pipelined, and optimal local
          on-chip memory reuse is attempted, in order to minimize the loss in bandwidth, associated with external memory
          interaction. "
        * "Uniform streaming, where one kernel function is applied to all elements in the stream, is typical."

    * Streaming Platform

    * Event Stream Platform


  + Broker
    * "A broker is a server that routes published messages to subscribers."

  + Pub/Sub
    * https://cloud.google.com/solutions/event-driven-architecture-pubsub
      * "This document discusses the differences between on-premises message-queue-driven architectures and the
        cloud-based, event-driven architectures that are implemented on Pub/Sub"

        * image source: google.com
            * ![](https://cloud.google.com/solutions/images/event-driven-architecture-pubsub-1-comparison-overview.svg)

    * https://cloud.google.com/pubsub/architecture


  + Real Time Streaming Protocol (RTSP)
    * https://en.wikipedia.org/wiki/Real_Time_Streaming_Protocol
      * "a network control protocol designed for use in entertainment and communications systems to control streaming
        media servers."

- Useful distinction..._?_
  + real-time data streams 
  + messaging



## Solution Citations/References

### Advanced Messaging Queue Protocol (AMQP)
- https://www.amqp.org/
  * "The Advanced Message Queuing Protocol (AMQP) is an open standard for passing business messages between applications
    or organizations. "

- https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol
  * "The Advanced Message Queuing Protocol (AMQP) is an open standard application layer protocol for message-oriented
     middleware. The defining features of AMQP are message orientation, queuing, routing (including point-to-point and
     publish-and-subscribe), reliability and security."
  * "Previous standardizations of middleware have happened at the API level (e.g. JMS) and were focused on
    standardizing programmer interaction with different middleware implementations, rather than on providing
    interoperability between multiple implementations.[2] Unlike JMS, which defines an API and a set of behaviors that
    a messaging implementation must provide, AMQP is a wire-level protocol. A wire-level protocol is a description of
    the format of the data that is sent across the network as a stream of bytes."
  * "The link protocol transfers messages between two nodes but assumes very little as to what those nodes are or how
    they are implemented. "
  * "A key category is those nodes used as a _*rendezvous point*_ between senders and receivers of messages (e.g. queues
     or topics). The AMQP specification calls such nodes distribution nodes and codifies some common behaviors."



### Amazon Kinesis
- https://aws.amazon.com/kinesis/
  + https://aws.amazon.com/kinesis/data-streams/
  + source: amazon.com
    * ![](https://d1.awsstatic.com/Products/product-name/diagrams/product-page-diagram_Amazon-Kinesis-Data-Streams.074de94302fd60948e1ad070e425eeda73d350e7.png)

- https://docs.aws.amazon.com/streams/latest/dev/introduction.html


### Amazon Simple Queue Service (SQS)
- https://en.wikipedia.org/wiki/Amazon_Simple_Queue_Service


### Apache ActiveMQ
- https://en.wikipedia.org/wiki/Apache_ActiveMQ


### Apache Flink
- https://flink.apache.org/
  + source: flink.apache.org
    * ![](https://flink.apache.org/img/flink-home-graphic.png)

- https://ci.apache.org/projects/flink/flink-docs-master/

- https://en.wikipedia.org/wiki/Apache_Flink
  * "an open-source, unified stream-processing and batch-processing framework"
  * "The core of Apache Flink is a distributed streaming data-flow engine written in Java and Scala."
  * "Flink executes arbitrary dataflow programs in a data-parallel and pipelined (hence task parallel) manner."
  * "Flink's pipelined runtime system enables the execution of bulk/batch and stream processing programs"
  * "Flink provides a high-throughput, low-latency streaming engine[8] as well as support for event-time processing and
    state management."
  * "Flink applications are fault-tolerant in the event of machine failure and support exactly-once semantics."
  * "Flink does not provide its own data-storage system, but provides data-source and sink connectors to systems such as
    Amazon Kinesis, Apache Kafka, HDFS, Apache Cassandra, and ElasticSearch"
  * "Apache Flink's dataflow programming model provides *event-at-a-time processing on both finite and infinite* datasets."
  * "Flink programs consist of streams and transformations"
  * "Conceptually, a stream is a (potentially never-ending) flow of data records, and a transformation is an operation
    that takes one or more streams as input, and produces one or more output streams as a result."
  * "Apache Flink includes two core APIs: a DataStream API for bounded or unbounded streams of data and a DataSet API
    for bounded data sets."
  * "Flink programs are mapped to streaming dataflows. Every Flink dataflow starts with one or more sources (a data
    input, e.g., a message queue or a file system) and ends with one or more sinks (a data output, e.g., a message
    queue, file system, or database)"
  * "Flink offers ready-built source and sink connectors with Apache Kafka, Amazon Kinesis, HDFS, Apache Cassandra, and
    more"
  * "Apache Flink includes a lightweight fault tolerance mechanism based on distributed checkpoints."
  * "A checkpoint is an automatic, asynchronous snapshot of the state of an application and the position in a source
    stream. In the case of a failure, a Flink program with checkpointing enabled will, upon recovery, resume processing
    from the last completed checkpoint, ensuring that Flink maintains exactly-once state semantics within an
    application"
  * "Flink also includes a mechanism called savepoints, which are manually-triggered checkpoints.[21] A user can
    generate a savepoint, stop a running Flink program, then resume the program from the same application state and
    position in the stream."
  * "Savepoints enable updates to a Flink program or a Flink cluster without losing the application's state ."


### Apache Heron
- https://en.wikipedia.org/wiki/Apache_Heron
  + "Apache Heron is a distributed stream processing engine developed at Twitter. According to the creators at Twitter,
    the scale and diversity of Twitter data has increased, and Heron is a real-time analytics platform to process
    streaming. It was introduced at the SIGMOD 2015.[2] Heron is API compatible with Apache Storm."



### Apache Pulse


### Apache Qpid

### Apache Spark 
- https://spark.apache.org/
  * "Apache Spark™ is a unified analytics engine for large-scale data processing."
  * "Apache Spark achieves high performance for both batch and streaming data, using a state-of-the-art DAG scheduler, a
    query optimizer, and a physical execution engine. "

- https://spark.apache.org/streaming/

- https://spark.apache.org/docs/latest/
  + https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html
    * "Structured Streaming is a scalable and fault-tolerant stream processing engine built on the Spark SQL engine. You
      can express your streaming computation the same way you would express a batch computation on static data."
    * "Since Spark 2.0, DataFrames and Datasets can represent static, bounded data, as well as streaming, unbounded
      data."
    * "imilar to static Datasets/DataFrames, you can use the common entry point SparkSession to create streaming DataFrames/Datasets from streaming sources, and apply the same operations on them as static DataFrames/Datasets."
        * https://spark.apache.org/docs/latest/sql-programming-guide.html
    * https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html#creating-streaming-dataframes-and-streaming-datasets
      * Input Sources (builtin):
        * File source
        * Kafka source
        * Socket source (for testing)
        * Rate source (for testing) 
      * "Some sources are not fault-tolerant because they do not guarantee that data can be replayed using checkpointed
        offsets after a failure."
    * https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html#operations-on-streaming-dataframesdatasets
      * "You can apply all kinds of operations on streaming DataFrames/Datasets – ranging from untyped, SQL-like
        operations (e.g. select, where, groupBy), to typed RDD-like operations (e.g. map, filter, flatMap). See the SQL
        programming guide for more details. Let’s take a look at a few example operations that you can use."

- https://en.wikipedia.org/wiki/Apache_Spark
  + "an open-source unified analytics engine for large-scale data processing. Spark provides an interface for
    programming entire clusters with implicit data parallelism and fault tolerance. Originally developed at the
    University of California, Berkeley's AMPLab, the Spark codebase was later donated to the Apache Software Foundation,
    which has maintained it since."
  + "Apache Spark has its architectural foundation in the resilient distributed dataset (RDD), a read-only multiset of
    data items distributed over a cluster of machines, that is maintained in a fault-tolerant way"
  + "as of Spark 2.x use of the Dataset API is encouraged"
  + "Spark Core is the foundation of the overall project. It provides distributed task dispatching, scheduling, and
    basic I/O functionalities, exposed through an application programming interface (for Java, Python, Scala, .NET[16]
    and R) centered on the RDD abstraction (the Java API is available for other JVM languages, but is also usable for
    some other non-JVM languages that can connect to the JVM, such as Julia"
  + "This interface mirrors a functional/higher-order model of programming: a "driver" program invokes parallel
    operations such as map, filter or reduce on an RDD by passing a function to Spark, which then schedules the
    function's execution in parallel on the cluster"
  + "Spark Streaming uses Spark Core's fast scheduling capability to perform streaming analytics. It ingests data in
    mini-batches and performs RDD transformations on those mini-batches of data. This design enables the same set of
    application code written for batch analytics to be used in streaming analytics, thus facilitating easy
    implementation of lambda architecture."
  + "However, this convenience comes with the penalty of latency equal to the mini-batch duration. Other streaming data
    engines that process event by event rather than in mini-batches include Storm and the streaming component of Flink"
  + "Spark Streaming has support built-in to consume from Kafka, Flume, Twitter, ZeroMQ, Kinesis, and TCP/IP sockets."
  + "*In Spark 2.x, a separate technology based on Datasets, called Structured Streaming, that has a higher-level interface is also provided to support streaming*."


### Apache Storm
- https://storm.apache.org/
  + "Apache Storm is a free and open source distributed realtime computation system. Apache Storm makes it easy to
    reliably process unbounded streams of data, doing for realtime processing what Hadoop did for batch processing"

- https://storm.apache.org/releases/2.2.0/index.html
  + https://storm.apache.org/releases/2.2.0/Concepts.html
    * "The stream is the core abstraction in Storm. A stream is an unbounded sequence of tuples that is processed and
      created in parallel in a distributed fashion"
    * "A spout is a source of streams in a topology."
    * "All processing in topologies is done in bolts. Bolts can do anything from filtering, functions, aggregations,
      joins, talking to databases, and more."
    * "Part of defining a topology is specifying for each bolt which streams it should receive as input. A stream
      grouping defines how that stream should be partitioned among the bolt's tasks."
    * "There are eight built-in stream groupings in Storm, and you can implement a custom stream grouping by
      implementing the CustomStreamGrouping interface"
        * Shuffle grouping
        * Fields grouping
        * Partial Key grouping
        * All grouping
        * Global grouping
        * None grouping
        * Direct grouping
        * Local or shuffle grouping
    * "Each spout or bolt executes as many tasks across the cluster. Each task corresponds to one thread of execution, and stream groupings define how to send tuples from one set of tasks to another set of tasks"
    * "Topologies execute across one or more worker processes. Each worker process is a physical JVM and executes a
      subset of all the tasks for the topology."
    * "Storm guarantees that every spout tuple will be fully processed by the topology. "
  + https://storm.apache.org/releases/2.2.0/Guaranteeing-message-processing.html
    * "Storm offers several different levels of guaranteed message processing, including best effort, at least once, and
      exactly once through Trident."

- https://en.wikipedia.org/wiki/Apache_Storm
  + " a distributed stream processing computation framework written predominantly in the Clojure programming language."
  + "It uses custom created "spouts" and "bolts" to define information sources and manipulations to allow batch,
    distributed processing of streaming data."
  + "A Storm application is designed as a "topology" in the shape of a directed acyclic graph (DAG) with spouts and
    bolts acting as the graph vertices."
  + "*Edges on the graph are named streams* and direct data from one node to another"
  + "Together, the topology acts as a data transformation pipeline."
  + _"At a superficial level the general topology structure is similar to a MapReduce job, with the main difference being that data is processed in real time as opposed to in individual batches."_
  + "Additionally, Storm topologies run indefinitely until killed, _while a MapReduce job DAG must eventually end_"
  + "Storm has three critical components: Topology, Stream, and Spout. Topology is a network made of Stream and Spout.
    Stream is an unbounded pipeline of tuples and Spout is the source of the data streams which converts the data into
    the tuple of streams and sends to the bolts to be processed"


### Azure Stream Analytics
- https://azure.microsoft.com/en-us/services/stream-analytics/
  + "Serverless real-time analytics, from the cloud to the edge"

- https://azure.microsoft.com/en-us/services/stream-analytics/#documentation
  + https://docs.microsoft.com/en-us/azure/stream-analytics/stream-analytics-introduction
    * "Azure Stream Analytics is a real-time analytics and complex event-processing engine that is designed to analyze
      and process high volumes of fast streaming data from multiple sources simultaneously. Patterns and relationships
      can be identified in information extracted from a number of input sources including devices, sensors,
      clickstreams, social media feeds, and applications.":
    * "... examples of when you can use Azure Stream Analytics:"
      * "Analyze real-time telemetry streams from IoT devices"
      * "Web logs/clickstream analytics"
      * "Geospatial analytics for fleet management and driverless vehicle"
      * "Remote monitoring and predictive maintenance of high value assets"
      * "Real-time analytics on Point of Sale data for inventory control and anomaly detection"


### Google Dataflow 
- https://cloud.google.com/dataflow/
  + "Unified stream and batch data processing that's serverless, fast, and cost-effective."


- https://en.wikipedia.org/wiki/Google_Cloud_Dataflow
  + "Google Cloud Dataflow is a fully managed service for executing Apache Beam pipelines within the Google Cloud
    Platform ecosystem. "


### IBM MQ


### IBM Stream
- https://www.ibm.com/cloud/streaming-analytics

- https://ibmstreams.github.io/
  + https://ibmstreams.github.io/tutorials/

- https://developer.ibm.com/technologies/analytics/articles/introduction-ibm-streams/
  + image source: ibm.com
    * ![](https://developer.ibm.com/developer/default/articles/introduction-ibm-streams/images/stream-objects.png)


### JMS


### Kafka 
- https://en.wikipedia.org/wiki/Apache_Kafka
  + _" a framework implementation of a software bus using stream-processing."_
  + _"aims to provide a unified, high-throughput, low-latency platform for handling real-time data feeds."_
  + _"Apache Kafka is based on the commit log, and it allows users to subscribe to it and publish data to any number of systems or real-time applications"_
  + _"Kafka stores key-value messages that come from arbitrarily many processes called producers."_ 
  + _"The data can be partitioned into different "partitions" within different "topics". Within a partition, messages are strictly ordered by their offsets (the position of a message within a partition), and indexed and stored together with a timestamp."_
  + _"Other processes called "consumers" can read messages from partitions."_ 
  + _"Kafka runs on a cluster of one or more servers (called brokers), and the partitions of all topics are distributed across the cluster nodes. Additionally, partitions are replicated to multiple brokers. This architecture allows Kafka to deliver massive streams of messages in a fault-tolerant fashion and has allowed it to replace some of the conventional messaging systems like Java Message Service (JMS), Advanced Message Queuing Protocol (AMQP), etc. "_
  + There are five major APIs in Kafka:
    * Producer API – Permits an application to publish streams of records.
    * Consumer API – Permits an application to subscribe to topics and processes streams of records.
    * Connector API – Executes the reusable producer and consumer APIs that can link the topics to the existing applications.
    * Streams API – This API converts the input streams to output and produces the result.
    * Admin API – used to manage Kafka topics, brokers and other Kafka objects.

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



### Message Queue Telemtry Trasnport (MQTT)
- https://mqtt.org/
  * "MQTT is an OASIS standard messaging protocol for the Internet of Things (IoT). It is designed as an extremely
    lightweight publish/subscribe messaging transport that is ideal for connecting remote devices with a small code
    footprint and minimal network bandwidth. MQTT today is used in a wide variety of industries, such as automotive,
    manufacturing, telecommunications, oil and gas, etc."
  * FAQ: "MQTT is an OASIS standard for IoT connectivity. It is a publish/subscribe, extremely simple and lightweight
    messaging protocol, designed for constrained devices and low-bandwidth, high-latency or unreliable networks. The
    design principles are to minimise network bandwidth and device resource requirements whilst also attempting to
    ensure reliability and some degree of assurance of delivery. These principles also turn out to make the protocol
    ideal of the “Internet of Things” world of connected devices, and for mobile applications where bandwidth and
    battery power are at a premium."

- https://en.wikipedia.org/wiki/MQTT
  * "a lightweight, publish-subscribe network protocol that transports messages between devices. The protocol usually
    runs over TCP/IP; however, any network protocol that provides ordered, lossless, bi-directional connections can
    support MQTT."
  * "defines two types of network entities: a message broker and a number of clients."
  * "An MQTT broker is a server that receives all messages from the clients and then routes the messages to the
    appropriate destination clients."
  * "An MQTT client is any device (from a micro controller up to a fully-fledged server) that runs an MQTT library and
    connects to an MQTT broker over a network."
  * "Information is organized in a hierarchy of topics. When a publisher has a new item of data to distribute, it sends
    a control message with the data to the connected broker. *The broker then distributes the information to any clients
    that have subscribed to that topic*."
  * "The publisher does not need to have any data on the number or locations of subscribers, and subscribers, in turn,
    do not have to be configured with any data about the publishers."
  * "If a broker receives a message on a topic for which there are no current subscribers, the broker discards the
    message unless the publisher of the message designated the message as a retained message. A retained message is a
    normal MQTT message with the retained flag set to true. The broker stores the last retained message and the
    corresponding QoS for the selected topic. Each client that subscribes to a topic pattern that matches the topic of
    the retained message receives the retained message immediately after they subscribe. *The broker stores only one
    retained message per topic*."
  * "A minimal MQTT control message can be as little as two bytes of data. *A control message can carry nearly 256 megabytes of data if needed.*"
  * "MQTT sends connection credentials in plain text format and does not include any measures for security or authentication. This can be provided by using TLS to encrypt and protect the transferred information against interception, modification or forgery."
  * "The default unencrypted MQTT port is 1883. The encrypted port is 8883"



### Microsoft Message Queuing (MSMQ)
- https://en.wikipedia.org/wiki/Microsoft_Message_Queuing



### NATS 
- https://en.wikipedia.org/wiki/NATS_Messaging



### Oracle Messaging Cloud Service 


### RabbitMQ
- https://www.rabbitmq.com/

- https://www.rabbitmq.com/documentation.html

- https://www.rabbitmq.com/manpages.html

- https://en.wikipedia.org/wiki/RabbitMQ
  * "an open-source message-broker software (sometimes called message-oriented middleware) that originally
    implemented the Advanced Message Queuing Protocol (AMQP) and has since been extended with a plug-in architecture to
    support Streaming Text Oriented Messaging Protocol (STOMP), MQ Telemetry Transport (MQTT), and other protocols."



### TIBCO Enterprise Message Service 



### ZeroMQ


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


