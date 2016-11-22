# spark-kafka
Combines spark and kafka into a single development container
Suited for development or single node testing.

Versions:
* Spark Version 1.6.3 
* Hadoop Version 2.6
* Kafka Version 0.8.2.2

Features:
* Starts Spark Master
* Starts Spark Client
* Starts Kafka & Zookeeper
* Keeps the container alive forever
* Ports are exposed

To use spark-kafka for local development:
```
docker run --name sparfka -d -p 8080:8080 -p 8081:8081 -p 7077:7077 -p 9001:9001 -p 2181:2181 -p 9092:9092 starofall/spark-kafka-standalone
```

If you want to link it to another container just use:
```
docker run --name sparfka -d starofall/spark-kafka-standalone
```
