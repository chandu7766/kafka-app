# kafka-app
## Commands used:

1)This command is used to start the Zookeeper service
``.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties `` 

2)This command is used to start Kafka service
`` .\bin\windows\kafka-server-start.bat .\config\server.properties ``

3)This command is used to craete topic in kafka 
`` .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic Gampa-testing-topic``

4)This command is used to list the created topics
``.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list ``

5)This command is used to run kafka producer
``.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic Gampa-testing-topic``

6)This command is used to run consumer
``.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic Gampa-testing-topic --from-beginning ``
