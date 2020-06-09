# Docker Image Packaging for Python

## 3.8.2-XalvistackY - TBC

### Major Changes

  - Replace `tini` with `catatonit`
  - Rename `post_tasks.yml` as `side_effect.yml`

## 3.8.2-4alvistack4 - 2020-03-05

### Major Changes

  - Revamp with Molecule and `docker commit`
  - Consolidate molecule tests into `default` (noop)
  - Hotfix for systemd

## 3.8.1-3alvistack1 - 2020-01-15

### Major Changes

  - Replace `dumb-init` with `tini`, as like as `docker --init`
  - Include release specific vars and tasks
  - Support Python 3.6/3.7/3.8 with Ubuntu PPA

## 3.6.9-2alvistack1 - 2020-01-07

  - Ubuntu 18.04 based
  - Handle ENTRYPOINT with dumb-init
  - Self initialize with Ansible, by dogfooding with Ansible Playbook
