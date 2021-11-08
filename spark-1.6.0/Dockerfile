FROM ubuntu

RUN \
  apt-get update && \
  apt-get install -y wget

RUN apt-get install -y default-jdk
RUN apt-get install -y scala

RUN wget https://archive.apache.org/dist/spark/spark-1.6.0/spark-1.6.0-bin-hadoop2.6.tgz
RUN tar -xvf spark-1.6.0-bin-hadoop2.6.tgz
RUN mv spark-1.6.0-bin-hadoop2.6 /usr/local/

ENV SPARK /usr/local/spark-1.6.0-bin-hadoop2.6/bin/spark-shell

VOLUME /home/mauricio/docker-volumes/spark-1.6.0/ /home/spark-1.6.0/