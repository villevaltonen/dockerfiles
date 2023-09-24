FROM openjdk:11-jre-slim-bullseye

ARG SCALA_VERSION=2.13
ARG KAFKA_VERSION=3.0.0

RUN apt-get update
RUN apt-get install wget curl -y

RUN wget https://dlcdn.apache.org/kafka/${KAFKA_VERSION}/kafka_${SCALA_VERSION}-${KAFKA_VERSION}.tgz
RUN tar -xzf kafka_${SCALA_VERSION}-${KAFKA_VERSION}.tgz
