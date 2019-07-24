FROM gizmotronic/oracle-java8

ENV LANG C.UTF-8

ENV TZ 'Asia/Shanghai'
RUN echo $TZ > /etc/timezone \
    && apt-get update \
    && apt-get install -y tzdata \
    && rm /etc/localtime \
    && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime \
    && dpkg-reconfigure -f noninteractive tzdata \
    && apt-get clean