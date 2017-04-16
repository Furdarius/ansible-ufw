# Ansible Role: SSH
[![Build Status](https://travis-ci.org/Furdarius/ansible-ufw.svg?branch=master)](https://travis-ci.org/Furdarius/ansible-ufw)

Enable [UFW](https://help.ubuntu.com/community/UFW) on remote machine

## Install

```bash
ansible-galaxy install Furdarius.ufw
```

## Variables

All variables can be found in [defaults/main.yml](https://github.com/Furdarius/ansible-ufw/blob/master/defaults/main.yml)

## Playbook example

```yaml
---
- hosts: all
  become: true
  roles:
    - ufw
  vars:
    ssh_port: 2222
```
