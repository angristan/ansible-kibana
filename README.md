# Ansible role for Kibana

[![CircleCI](https://circleci.com/gh/angristan/ansible-kibana.svg?style=svg)](https://circleci.com/gh/angristan/ansible-kibana)

This is a simple role that will install Kibana on Debian/Ubuntu from the official APT repo.

The configuration (`kibana.yml`) is done via variables (see `defaults/main.yml`).

## Sample playbook

```yaml
---

- hosts: myhost
  roles:
    - name: kibana
      tags: kibana
  vars:
    kibana_server_host: 0.0.0.0
    kibana_server_name: My Kibana
```
