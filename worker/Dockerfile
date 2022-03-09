FROM spark-base:latest

COPY start-worker.sh /

ENV SPARK_MASTER="spark://spark-master:7077"
ENV SPARK_HOME="/spark"

ENV SPARK_WORKER_CORES=1
ENV SPARK_WORKER_MEMORY=2g

RUN chmod +x /start-worker.sh

CMD ["/bin/bash", "/start-worker.sh"]

