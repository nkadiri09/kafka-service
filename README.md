# kafka-service setup

## Setup Zookeeper properties:
Add the log directory to /tmp/zookeeper/logs
and add KAFKA_HOME

to run zookeeper:

%KAFKA_HOME%\bin\windows\zookeeper-server-start.bat %KAFKA_HOME%\etc\kafka\zookeeper.properties

To run kafka server:

# Kafka-server:

to run more instances of Kafka changes 3 things

Setup Broker id to a unique number
broker.id=1 

Have a different port nukber to each server in local
listeners=PLAINTEXT://:9093

Have a different logs to each kafka serve
log.dirs=/tmp/kafka-logs-1

