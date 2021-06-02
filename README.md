KAFKA DOCKER CONF

---

### Introduction:

Docker environment and config files for KAFKA BROKER

#

### Tech Stack:

1. Apache Kafka
2. Docker
3. Zookeeper
4. Kafdrop

#

### How to configure 

1. Clone the repository on the desired machine
2. Edit the docker-compose file appropriately
5. run sudo docker-compose up -d to start the containers 

### Caveats
Run atleast 3 brokers or else edit the KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR to 1 or else the consumers won't be able to connect
Make sure you understand the listeners configuration and expose ports appropriately

### References
- Basic configuration reference [Confluent - Docker Configuration Parameters](https://docs.confluent.io/platform/current/installation/docker/config-reference.html)
- Connectivity [Why can't I connect to Kafka](https://www.confluent.io/blog/kafka-client-cannot-connect-to-broker-on-aws-on-docker-etc/)
- Kafka Listeners [Kafka listeners explained](https://www.confluent.io/blog/kafka-listeners-explained/)

