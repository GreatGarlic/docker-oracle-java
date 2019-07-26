#
# Oracle Java 9 Dockerfile
#
# https://github.com/cogniteev/docker-oracle-java
# https://github.com/cogniteev/docker-oracle-java/tree/master/oracle-java9
#

# Pull base image.
FROM ubuntu:16.04

ARG version=9.0.4-1~webupd8~0

# Install Java.
# RUN \
#   apt-get update && \
#   apt-get install -y software-properties-common && \
#   #echo oracle-java9-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
#   add-apt-repository -y ppa:linuxuprising/java && \
#   apt-get update && \
#   apt-get install -y oracle-java11-installer && \
#   rm -rf /var/lib/apt/lists/* && \
#   rm -rf /var/cache/oracle-jdk11-installer

RUN apt update \
    && apt upgrade \
    && apt-get install -y software-properties-common \
    && add-apt-repository ppa:linuxuprising/java \
    && echo debconf shared/accepted-oracle-license-v1-1 select true | debconf-set-selections \
    && echo debconf shared/accepted-oracle-license-v1-1 seen true | debconf-set-selections \
    && apt update \
    && apt-get install oracle-java11-installer \
    && apt-get install oracle-java11-set-default 
# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-11-oracle

# Define default command.
CMD ["bash"]
