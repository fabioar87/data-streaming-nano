# Data Streaming Repository

Kafka in action and further optional research links:

- [Confluent kafka python library doc](https://docs.confluent.io/current/clients/confluent-kafka-python/)
- [Kafka command line tools](https://github.com/apache/kafka/tree/trunk/bin)
- [Kafka topics, producers and consumers](https://kafka.apache.org/documentation/#intro_topics)
- [Why does kafka need zookeeper?](https://www.cloudkarafka.com/blog/2018-07-04-cloudkarafka_what_is_zookeeper.html)
- [IBM Kafka architecture](https://ibm-cloud-architecture.github.io/refarch-eda/technology/kafka-overview/)
- [Setup Kafka on Kubernetes](https://phoenixnap.com/kb/kafka-on-kubernetes)

## The Number of Partitions

This Confluent article indicates how to plan the numnber of partitions.

- [Number of partitions](https://www.confluent.io/blog/how-choose-number-topics-partitions-kafka-cluster/)

## Best pratices and anti patterns

_Kafka_ can create topics automaticaly, but it is not recommended. The best practice is create them manually. It is possible create topic using script code, like _sh_ or even _terraform_ and _ansible_.

_Terraform_ can control the topic creation and also the ACL management.

## Installed Packages Locally

## Distributed Systems Reading Group

- _MIT_ [group link](http://dsrg.pdos.csail.mit.edu/papers/)

## Compression

An article about the pros and cons, [here is the link](https://blog.cloudflare.com/squeezing-the-firehose/)

**Here Is a question**: what is network overhead?

## Kafka Local Cluster Config

[Kind](https://kind.sigs.k8s.io/) is used to create the local kafka cluster (using the kafka on kubernetes model).Kind command to create the cluster:

```
$ kind create cluster --config YAML_FILE --name CLUSTER_NAME
```

The local cluster is configured with 3 nodes (1 control plane and two worker nodes)
