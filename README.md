# Docker Image Packaging for Postfix

<a href="https://alvistack.com" title="AlviStack" target="_blank"><img src="/alvistack.svg" height="75" alt="AlviStack"></a>

[![GitLab pipeline
status](https://img.shields.io/gitlab/pipeline/alvistack/docker-postfix/master)](https://gitlab.com/alvistack/docker-postfix/-/pipelines)
[![GitHub
tag](https://img.shields.io/github/tag/alvistack/docker-postfix.svg)](https://github.com/alvistack/docker-postfix/tags)
[![GitHub
license](https://img.shields.io/github/license/alvistack/docker-postfix.svg)](https://github.com/alvistack/docker-postfix/blob/master/LICENSE)
[![Docker
Pulls](https://img.shields.io/docker/pulls/alvistack/postfix-3.8.svg)](https://hub.docker.com/r/alvistack/postfix-3.8)

This image contains an installation of the Postfix mail transport agent.

Learn more about Postfix: <http://www.postfix.org/>

## Supported Tags and Respective Packer Template Links

- [`alvistack/postfix-3.8`](https://hub.docker.com/r/alvistack/postfix-3.8)
  - [`packer/docker-3.8/packer.json`](https://github.com/alvistack/docker-postfix/blob/master/packer/docker-3.8/packer.json)

## Overview

This Docker container makes it easy to get an instance of postfix up and
running.

Based on [Official Ubuntu Docker
Image](https://hub.docker.com/_/ubuntu/) with some minor hack:

- Packaging by Packer Docker builder and Ansible provisioner in single
  layer
- Handle `ENTRYPOINT` with
  [catatonit](https://github.com/openSUSE/catatonit)

### Quick Start

Start Postfix:

    # Pull latest image
    docker pull alvistack/postfix-3.8

    # Run as detach
    docker run \
        -itd \
        --name postfix \
        --publish 2525:25 \
        alvistack/postfix-3.8

**Success**. Postfix is now available on port `2525`.

## Versioning

### `YYYYMMDD.Y.Z`

Release tags could be find from [GitHub
Release](https://github.com/alvistack/docker-postfix/tags) of this
repository. Thus using these tags will ensure you are running the most
up to date stable version of this image.

### `YYYYMMDD.0.0`

Version tags ended with `.0.0` are rolling release rebuild by [GitLab
pipeline](https://gitlab.com/alvistack/docker-postfix/-/pipelines) in
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
