# kafka-demo

Kafka Tutorial - **[Spring Boot Microservices](https://www.youtube.com/watch?v=SqVfCyfCJqw
)**

Steps:
1. Download and run kafka locally
    - **[kafka quick start](https://kafka.apache.org/quickstart)**
    - bin/zookeeper-server-start.sh config/zookeeper.properties
    - bin/kafka-server-start.sh config/server.properties
2. Spring Boot to create and sent Topic to Kafka (commandLineRunner)
3. Kafka CLI to receive Topic
    - bin/kafka-console-consumer.sh --topic luluTopic --from-beginning --bootstrap-server localhost:9092
4. Sprint Boot to consume Topic (KafkaListners)
   - to listen to the real-time Topic
5. RESTfull API 
    - to publish a Topic via POST
    -POST http://localhost:8080/api/v1/messages
        Content-Type: application/json

        {
          "message": "rest aaa"
        }
    - ![image](https://user-images.githubusercontent.com/89087221/189471103-f409532c-7821-4b32-9a24-acd7d72419aa.png)

