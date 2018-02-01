# Supported tags and respective `Dockerfile` links

* `java8`, `latest`, `8u161` [(Dockerfile)](https://github.com/gizmotronic/docker-oracle-java/blob/master/oracle-java8/Dockerfile)
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
