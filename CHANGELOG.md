# Docker Image Packaging for Postfix

## YYYYMMDD.Y.Z - TBC

### Major Changes

  - Upgrade minimal Ansible community package support to 4.10

## 20211020.1.1 - 2021-10-20

### Major Changes

  - Install dependencies with package manager
  - Upgrade minimal Ansible community package support to 4.7.0

## 20210718.1.1 - 2021-07-18

### Major Changes

  - Upgrade minimal Ansible community package support to 4.2.0

## 20210602.1.1 - 2021-06-02

### Major Changes

  - Upgrade minimal Ansible support to 4.0.0

## 20210313.1.1 - 2021-03-13

### Major Changes

  - Bugfix [ansible-lint `namespace`](https://github.com/ansible-community/ansible-lint/pull/1451)
  - Bugfix [ansible-lint `no-handler`](https://github.com/ansible-community/ansible-lint/pull/1402)
  - Bugfix [ansible-lint `unnamed-task`](https://github.com/ansible-community/ansible-lint/pull/1413)
  - Change GIT tag as per Vagrant Box naming and versioning limitation

## 3.4.13-4alvistack8 - 2020-12-09

### Major Changes

  - Migrate from Travis CI to GitLab CI
  - Revamp with Packer

## 3.4.13-4alvistack5 - 2020-10-14

### Major Changes

  - Refine Molecule matrix

## 3.4.13-4alvistack2 - 2020-08-26

### Major Changes

  - Upgrade minimal Ansible Lint support to 4.3.2
  - Upgrade Travis CI test as Ubuntu Focal based
  - Upgrade minimal Ansible support to 2.10.0

## 3.4.10-4alvistack1 - 2020-07-03

  - Ubuntu 20.04 based
  - Minimized `Dockerfile` for meta data definition
  - Provision by Ansible and Molecule Docker driver in single layer
  - Handle `ENTRYPOINT` with `catatonit`
