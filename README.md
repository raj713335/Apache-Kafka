# Apache-Kafka

# Download Apache Kafka 
```
https://kafka.apache.org/downloads
```

# Starting Kafka Zookeper 

```
C:\kafka_2.12-3.3.1>bin\windows\zookeeper-server-start.bat config\zookeeper.properties
C:\kafka_2.12-3.3.1>bin\windows\kafka-server-start.bat config\server.properties
```

# Creating a Topic

```
C:\kafka_2.12-3.3.1>bin\windows\kafka-topics.bat --create --topic test --partitions 1 --replication-factor 1 --bootstrap-server localhost:9092
```

# Kafka Console Producer 

```
C:\kafka_2.12-3.3.1>bin\windows\kafka-console-producer.bat --topic test --broker-list localhost:9092 < ..\data\sample1.csv
```

# Kafka Console Consumer 

```
C:\kafka_2.12-3.3.1>bin\windows\kafka-console-consumer.bat --topic test --bootstrap-server localhost:9092 --from-beginning
```
