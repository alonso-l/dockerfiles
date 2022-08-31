FROM ubuntu:14.04
LABEL MAINTAINER="Leonardo Alonso - https://github.com/alonso-l" 

ENV DEBIAN_FRONTEND noninteractive
COPY jdk-1_5_0_22-linux-amd64.bin /tmp/

SHELL ["/bin/bash", "-o", "pipefail", "-c"]
RUN echo yes|sh /tmp/jdk-1_5_0_22-linux-amd64.bin && \
    rm -rf /tmp/jdk-1_5_0_22-linux-amd64.bin

ENV JAVA_HOME /jdk1.5.0_22
ENV PATH /jdk1.5.0_22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
