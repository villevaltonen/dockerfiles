FROM openjdk:11-jre-slim-bullseye

RUN apt-get update
RUN apt-get install wget curl -y

RUN wget https://dlcdn.apache.org/kafka/3.0.0/kafka_2.13-3.0.0.tgz
RUN tar -xzf kafka_2.13-3.0.0.tgz