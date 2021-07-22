# Docker Image Packaging for Python

[![GitLab pipeline
status](https://img.shields.io/gitlab/pipeline/alvistack/docker-python/master)](https://gitlab.com/alvistack/docker-python/-/pipelines)
[![GitHub
release](https://img.shields.io/github/release/alvistack/docker-python.svg)](https://github.com/alvistack/docker-python/releases)
[![GitHub
license](https://img.shields.io/github/license/alvistack/docker-python.svg)](https://github.com/alvistack/docker-python/blob/master/LICENSE)
[![Docker
Pulls](https://img.shields.io/docker/pulls/alvistack/python-3.8.svg)](https://hub.docker.com/r/alvistack/python-3.8)

Python is an interpreted, interactive, object-oriented, open-source
programming language.

Learn more about Python: <https://www.python.org/>

## Supported Tags and Respective Packer Template Links

  - [`alvistack/python-3.8`](https://hub.docker.com/r/alvistack/python-3.8)
      - [`packer/docker-3.8/packer.json`](https://github.com/alvistack/docker-python/blob/master/packer/docker-3.8/packer.json)
  - [`alvistack/python-3.7`](https://hub.docker.com/r/alvistack/python-3.7)
      - [`packer/docker-3.7/packer.json`](https://github.com/alvistack/docker-python/blob/master/packer/docker-3.7/packer.json)
  - [`alvistack/python-3.6`](https://hub.docker.com/r/alvistack/python-3.6)
      - [`packer/docker-3.6/packer.json`](https://github.com/alvistack/docker-python/blob/master/packer/docker-3.6/packer.json)

## Overview

This Docker container makes it easy to get an instance of Python up and
running.

Based on [Official Ubuntu Docker
Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Packaging by Packer Docker builder and Ansible provisioner in single
    layer
  - Handle `ENTRYPOINT` with
    [catatonit](https://github.com/openSUSE/catatonit)

### Quick Start

For the `VOLUME` directory that is used to store the repository data
(amongst other things) we recommend mounting a host directory as a [data
volume](https://docs.docker.com/engine/tutorials/dockervolumes/#/data-volumes),
or via a named volume if using a docker version \>= 1.9.

Start Python:

    # Pull latest image
    docker pull alvistack/python-3.8
    
    # Run as detach
    docker run \
        -itd \
        --rm \
        --name python \
        alvistack/python-3.8 \
        python --version

## Versioning

### `YYYYMMDD.Y.Z`

Release tags could be find from [GitHub
Release](https://github.com/alvistack/docker-python/releases) of this
repository. Thus using these tags will ensure you are running the most
up to date stable version of this image.

### `YYYYMMDD.0.0`

Version tags ended with `.0.0` are rolling release rebuild by [GitLab
pipeline](https://gitlab.com/alvistack/docker-python/-/pipelines) in
weekly basis. Thus using these tags will ensure you are running the
latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY
    4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
