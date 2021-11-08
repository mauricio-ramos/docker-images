FROM ubuntu

RUN \
  apt-get update && \
  apt-get install -y wget

RUN apt-get install -y default-jdk
RUN apt-get install -y scala

RUN wget http://ftp.unicamp.br/pub/apache/spark/spark-2.4.7/spark-2.4.7-bin-hadoop2.7.tgz
RUN tar -xvf spark-2.4.7-bin-hadoop2.7.tgz
RUN mv spark-2.4.7-bin-hadoop2.7 /usr/local/

ENV SPARK-SHELL /usr/local/spark-2.4.7-bin-hadoop2.7/bin/spark-shell
ENV PYSPARK /usr/local/spark-2.4.7-bin-hadoop2.7/bin/spark-shell

VOLUME /home/mauricio/docker-volumes/spark-2.4.7/ /home/spark-2.4.7/
