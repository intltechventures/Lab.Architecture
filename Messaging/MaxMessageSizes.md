
# Maximum Message Sizes


## Message Queue Technologies

### SQS
- A notable limitation of SQS, for which I find many solution architect folks lack awareness:
- The maximum message size is 256KB (2GB is supported using the {Java | Python} Extended Client, which passes a reference to an S3 location).
  + https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/quotas-messages.html


### Kafka 
- Kafka (default): 1MB
  + https://www.confluent.io/learn/kafka-message-size-limit/


### ActiveMQ
- ActiveMQ: 100KiB
  + https://activemq.apache.org/components/artemis/documentation/latest/large-messages.html#large-messages


### HiveMQ
- HiveMQ (re: MQTT compliance): 256MB
  + "The max-packet-size value defines the largest MQTT packet size in bytes that HiveMQ accepts. The default max-packet-size value is set to the maximum packet size the MQTT protocol allows: 268,435,460 bytes (equivalent to 256 MB)."
  + https://docs.hivemq.com/hivemq/latest/user-guide/configuration.html#max-packet


### Google Pub/Sub
- Google Pub/Sub (re: data field): 10MB
  + https://cloud.google.com/pubsub/quotas
