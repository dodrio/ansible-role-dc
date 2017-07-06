# dc

[![Build Status](https://travis-ci.org/m31271n/ansible-role-dc.svg?branch=master)](https://travis-ci.org/m31271n/ansible-role-dc)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-m31271n.dc-blue.svg)](https://galaxy.ansible.com/m31271n/dc)

Ansible role to deploy containers via docker-compose.

## Requirements

+ `docker-compose`

## Role Variables

+ `dc_dest_dir`: `/srv/example`
+ `dc_compose_file_src`: `'{{ playbook_dir }}/files/dc/docker-compose.yml'`
+ `dc_compose_file_dest`: `'{{ dc_dest_dir }}/docker-compose.yml'`

## Dependencies

+ `m31271n.docker-compose`

## Example Playbook

```
- hosts: servers
  roles:
    - role: m31271n.dc
      dc_dest_dir: /srv/project
      dc_compose_file_src: '{{ playbook_dir }}/files/dc/project.yml'
```

* * *

<p align="center">Made with ❤ by <a href="http://index.m31271n.com">m31271n</a></p>
