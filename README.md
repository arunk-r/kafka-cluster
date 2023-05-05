# Kafka Cluster

Apache Kafka is a distributed open source system for publishing and subscribing to a large number of messages.

It enables developers to build applications that continuously produce and consume streams of data records using a message broker to route messages from publishers to subscribers.

## Key Features of Apache Kafka
- Low latency
- Seamless messaging functionality
- High Scalability
- High Fault Tolerance
- Multiple Integrations


## What is Kafka Clusters?
More than one kafka broker is called cluster. Clusters are user to manage the persistence and replication of the messages. If primary cluster goes down, other clusters can be used to deliver the message to service without any delay.

In a distributed system, a cluster is a collection of computers working together to achieve a shared goal.
Cluster consists of 
- brokers
- topics
- partitions

The primary objective is to keep workload equally among all replicas and partitions. Then main components are
- **Zookeeper**: it stores the consumer and cluster details and act like a Management Node. 
- **Broker**: Server is known as broker and serer is responsible to message storage (many other responsibilities)
- **Topics**: collections of messages belong to one name. Producers post message to topic and Consumers will consume. Topics are segmented into customizable number of sections called partitions. 
- **Producers**: producer sends or publishes message to the topic. When producer sends a message broker leader commits the log and increases record offset.
- **Consumers**: who read or consumes the message. We can configure consumer where to read message topic (```earliest```, ```latest```)
