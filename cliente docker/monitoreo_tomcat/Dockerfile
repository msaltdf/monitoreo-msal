FROM bitnami/jmx-exporter:latest

USER root
RUN apt-get update && \
    apt-get install -y iputils-ping telnet curl  && \
    rm -rf /var/lib/apt/lists/*
USER 1001