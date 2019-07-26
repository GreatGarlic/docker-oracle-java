FROM ubuntu:16.04

#Install Open JDK 8

ENV LANG C.UTF-8

ENV TZ 'Asia/Shanghai'

RUN apt-get update \
	&& echo $TZ > /etc/timezone \
    && apt-get install -y tzdata \
    && rm /etc/localtime \
    && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime \
    && dpkg-reconfigure -f noninteractive tzdata \
    && apt-get -y -o Dpkg::Options::="--force-overwrite" install openjdk-9-jdk \
	&& apt-get clean \
    && rm -rf /var/lib/apt/lists/*



ENV JAVA_HOME /usr/lib/jvm/java-9-openjdk-amd64
ENV PATH $JAVA_HOME/bin:$PATH