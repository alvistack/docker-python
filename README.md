# Docker Image Packaging for Python

[![Travis](https://img.shields.io/travis/alvistack/docker-python.svg)](https://travis-ci.org/alvistack/docker-python)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-python.svg)](https://github.com/alvistack/docker-python/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-python.svg)](https://github.com/alvistack/docker-python/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/python.svg)](https://hub.docker.com/r/alvistack/python/)

Python is an interpreted, interactive, object-oriented, open-source programming language.

Learn more about Python: <https://www.python.org/>

## Supported Tags and Respective `Dockerfile` Links

  - [`latest` (master/Dockerfile)](https://github.com/alvistack/docker-python/blob/master/Dockerfile)
  - [`3` (3/Dockerfile)](https://github.com/alvistack/docker-python/blob/3/Dockerfile)

## Overview

This Docker container makes it easy to get an instance of Python up and running.

### Quick Start

For the `VOLUME` directory that is used to store the repository data (amongst other things) we recommend mounting a host directory as a [data volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes), or via a named volume if using a docker version \>= 1.9.

Start Python:

    # Pull latest image
    docker pull alvistack/python
    
    # Run with built-in web server
    docker run \
        -itd \
        --rm \
        --name python \
        alvistack/python \
        python --version

## Versioning

The `latest` tag matches the most recent version of this repository. Thus using `alvistack/python:latest` or `alvistack/python` will ensure you are running the most up to date version of this image.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
