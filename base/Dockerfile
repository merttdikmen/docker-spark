FROM alpine:3.15

ENV SPARK_BASE_URL=https://archive.apache.org/dist/spark/
ENV SPARK_VERSION=3.2.1
ENV HADOOP_VERSION=3.2

RUN apk add --no-cache bash openjdk8 python3 py3-pip \
	&& wget ${SPARK_BASE_URL}/spark-${SPARK_VERSION}/spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz \
	&& tar -xvf spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz \
	&& mv spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION} spark \
	&& rm spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz

