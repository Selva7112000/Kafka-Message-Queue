# Kafka-Message-Queue
# Kafka Producer-Consumer Example in Golang

This project demonstrates a simple Kafka producer-consumer setup in Golang. The producer sends coffee orders to a Kafka topic, and the consumer processes these orders.


## Prerequisites

- Install [Docker](https://www.docker.com/)
- Install [Golang](https://go.dev/)
- Kafka 3.7.0 Docker Image

## Step 1: Run Apache Kafka

Pull and run the Kafka image using Docker:

```sh
docker pull apache/kafka:3.7.0
docker run -p 9092:9092 apache/kafka:3.7.0


curl -X POST http://localhost:3000/order -H "Content-Type: application/json" -d '{
  "customer_name": "John Doe",
  "coffee_type": "Espresso"
}'
