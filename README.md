# vagrant

[![Build Status](https://travis-ci.org/akostyrev/ansible-role-vagrant.svg?branch=master)](https://travis-ci.org/akostyrev/ansible-role-vagrant)

Installs vagrant

Requirements
------------

None

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml) for a list and description of
variables used in this role.

Example Playbook
----------------

```yaml
---
- hosts: all
  roles:
    - role: akostyrev.vagrant
      vagrant_validate_certs: "{{ false if ansible_virtualization_type == 'docker' else true }}"


```

License
-------

BSD

Author Information
------------------

Aleksandr Kostyrev
