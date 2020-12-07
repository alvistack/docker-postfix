# Docker Image Packaging for Postfix

[![Travis](https://img.shields.io/travis/com/alvistack/docker-postfix.svg)](https://travis-ci.com/alvistack/docker-postfix)
[![GitHub release](https://img.shields.io/github/release/alvistack/docker-postfix.svg)](https://github.com/alvistack/docker-postfix/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/docker-postfix.svg)](https://github.com/alvistack/docker-postfix/blob/master/LICENSE)
[![Docker Pulls](https://img.shields.io/docker/pulls/alvistack/postfix.svg)](https://hub.docker.com/r/alvistack/postfix/)

This image contains an installation of the Postfix mail transport agent.

Learn more about Postfix: <http://www.postfix.org/>

## Supported Tags and Respective Packer Template Links

  - [`3.4`, `latest`](https://github.com/alvistack/docker-postfix/blob/master/packer/docker-3.4/packer.json)

## Overview

This Docker container makes it easy to get an instance of postfix up and running.

Based on [Official Ubuntu Docker Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

  - Packaging by Packer Docker builder and Ansible provisioner in single layer
  - Handle `ENTRYPOINT` with [catatonit](https://github.com/openSUSE/catatonit)

### Quick Start

Start Postfix:

    # Pull latest image
    docker pull alvistack/postfix
    
    # Run as detach
    docker run \
        -itd \
        --name postfix \
        --publish 2525:25 \
        alvistack/postfix

**Success**. Postfix is now available on port `2525`.

## Versioning

### `alvistack/postfix:latest`

The `latest` tag matches the most recent [GitHub Release](https://github.com/alvistack/docker-postfix/releases) of this repository. Thus using `alvistack/postfix:latest` or `alvistack/postfix` will ensure you are running the most up to date stable version of this image.

### `alvistack/postfix:<version>`

The version tags are rolling release rebuild by [Travis](https://travis-ci.com/alvistack/docker-postfix) in weekly basis. Thus using these tags will ensure you are running the latest packages provided by the base image project.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
