
# Maximum Message Sizes


## Message Queue Technologies


### ActiveMQ
- https://activemq.apache.org/components/artemis/documentation/latest/large-messages.html#large-messages
  + ActiveMQ: 100KiB



### Azure Event Grid
- ?



### Azure Service Bus 
- ?



### Google Pub/Sub
- https://cloud.google.com/pubsub/quotas
  + Google Pub/Sub (re: data field): 10MB



### HiveMQ
- https://docs.hivemq.com/hivemq/latest/user-guide/configuration.html#max-packet
  + HiveMQ (re: MQTT compliance): 256MB
  + "The max-packet-size value defines the largest MQTT packet size in bytes that HiveMQ accepts. The default max-packet-size value is set to the maximum packet size the MQTT protocol allows: 268,435,460 bytes (equivalent to 256 MB)."



### Kafka 
- https://www.confluent.io/learn/kafka-message-size-limit/
  + Kafka (default): 1MB



### Solace
- ?



### SQS
- https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/quotas-messages.html
  + A notable limitation of SQS, for which I find many solution architect folks lack awareness:
  + The maximum message size is 256KB (2GB is supported using the {Java | Python} Extended Client, which passes a reference to an S3 location).
  + This extended library works only for synchronous clients.


