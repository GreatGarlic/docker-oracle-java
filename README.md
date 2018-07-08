# Oracle Java 8/9 on Ubuntu

To use these images, you must accept the [Oracle Binary Code License Agreement](http://www.oracle.com/technetwork/java/javase/terms/license/index.html) for Java SE.

## Supported tags and respective `Dockerfile` links

* `java8`, `latest`, `8u171` [(Dockerfile)](https://github.com/gizmotronic/docker-oracle-java/blob/master/oracle-java8/Dockerfile)
* `java10`, `10.0.1` [(Dockerfile)](https://github.com/gizmotronic/docker-oracle-java/blob/master/oracle-java10/Dockerfile)

## Deprecated tags

Java 9 has reached end of life.

* `java9`, `9.0.4` [(Dockerfile)](https://github.com/gizmotronic/docker-oracle-java/blob/master/oracle-java9/Dockerfile)

# Base Docker Image

* [ubuntu:16.04](https://registry.hub.docker.com/_/ubuntu/)

# Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/gizmotronic/oracle-java/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull gizmotronic/oracle-java`

### Usage

    docker run -it --rm gizmotronic/oracle-java

#### Run `java`

    docker run -it --rm gizmotronic/oracle-java java

#### Run `javac`

    docker run -it --rm gizmotronic/oracle-java javac

# LICENSE

MIT
