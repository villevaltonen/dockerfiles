FROM debian:bullseye-slim

ARG VERSION=0.89.1

RUN apt-get update && apt-get install wget -y

RUN wget https://github.com/gohugoio/hugo/releases/download/v$VERSION/hugo_${VERSION}_Linux-64bit.tar.gz
RUN tar -xzf hugo_${VERSION}_Linux-64bit.tar.gz

RUN adduser --disabled-password -u 1000 user
USER user