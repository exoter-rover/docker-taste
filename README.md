## Taste Dockerfile

![alt tag](exoter_docker_logo.jpg)

This repository contains **Dockerfile** of [Taste](http://taste.tuxfamily.org/wiki/index.php?title=Main_Page) for
[Docker](https://www.docker.com/)'s [automated
build](https://registry.hub.docker.com/u/jhidalgocarrio/taste/) published to the
public [Docker Hub Registry](https://registry.hub.docker.com/).

[![Build Status](https://travis-ci.org/jhidalgocarrio/docker-taste.svg?branch=master)](https://travis-ci.org/jhidalgocarrio/docker-taste)

### Base Docker Image

* [i386/ubuntu:14.04](https://hub.docker.com/r/i386/ubuntu/)


### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/jhidalgocarrio/taste/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull jhidalgocarrio/taste

    (alternatively, you can build an image from Dockerfile: `docker build -t jhidalgocarrio/taste:14.04 github.com/jhidalgocarrio/docker-taste )

### Usage

    docker run -it --rm jhidalgocarrio/taste:14.04

    You can also use the script file docker-run-taste.sh as following:
    sh docker-run-taste.sh . "-h docker"

    I needed to reinstall binfmt-support (my x86 host ubuntu)
    $sudo apt-get update
    $sudo apt-get install binfmt-support

    then run $sh docker-run-taste.sh . "-h docker" again
