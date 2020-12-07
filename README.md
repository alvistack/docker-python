# Docker Image Packaging for Python

[![Travis](https://img.shields.io/travis/com/alvistack/docker-python.svg)](https://travis-ci.com/alvistack/docker-python)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-python.svg)](https://github.com/alvistack/docker-python/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-python.svg)](https://github.com/alvistack/docker-python/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/python.svg)](https://hub.docker.com/r/alvistack/python/)

Python is an interpreted, interactive, object-oriented, open-source programming language.

Learn more about Python: <https://www.python.org/>

## Supported Tags and Respective Packer Template Links

  - [`3.8`, `latest`](https://github.com/alvistack/docker-pythong/blob/master/packer/docker-3.8/packer.json)
  - [`3.7`](https://github.com/alvistack/docker-pythong/blob/master/packer/docker-3.7/packer.json)
  - [`3.6`](https://github.com/alvistack/docker-pythong/blob/master/packer/docker-3.6/packer.json)

## Overview

This Docker container makes it easy to get an instance of Python up and running.

Based on [Official Ubuntu Docker Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Packaging by Packer Docker builder and Ansible provisioner in single layer
  - Handle `ENTRYPOINT` with [catatonit](https://github.com/openSUSE/catatonit)

### Quick Start

For the `VOLUME` directory that is used to store the repository data (amongst other things) we recommend mounting a host directory as a [data volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes), or via a named volume if using a docker version \>= 1.9.

Start Python:

    # Pull latest image
    docker pull alvistack/python
    
    # Run as detach
    docker run \
        -itd \
        --rm \
        --name python \
        alvistack/python \
        python --version

## Versioning

### `alvistack/python:latest`

The `latest` tag matches the most recent [GitHub Release](https://github.com/alvistack/docker-python/releases) of this repository. Thus using `alvistack/python:latest` or `alvistack/python` will ensure you are running the most up to date stable version of this image.

### `alvistack/python:<version>`

The version tags are rolling release rebuild by [Travis](https://travis-ci.com/alvistack/docker-python) in weekly basis. Thus using these tags will ensure you are running the latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
