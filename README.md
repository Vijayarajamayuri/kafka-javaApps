# kafka-javaApps

## Follow the steps below for running the Custom Consumer and Producer

### Start Zookeeper

.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties


### Start kafka server

.\bin\windows\kafka-server-start.bat .\config\server.properties

### Start the Consumer 

Here the topic name is test1 and group name is group1

 java -cp target/kafka-javaApps-1.0-SNAPSHOT-jar-with-dependencies.jar com.nwms.mayuri.kafka.CustomConsumer test1 group1
### Start the Producer

java -cp target/kafka-javaApps-1.0-SNAPSHOT-jar-with-dependencies.jar com.nwms.mayuri.kafka.CustomProducer test1

In the producer Terminal you will be prompted to enter the text that want to be encrypted. After you are done with entering the text you can find the encrypted text on the consumer terminal
