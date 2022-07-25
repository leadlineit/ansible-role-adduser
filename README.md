# Ansible Role Adduser

![Build Status](https://github.com/leadlineit/ansible-role-adduser/actions/workflows/ansible-galaxy-ci.yml/badge.svg)
[![Galaxy Role](https://img.shields.io/badge/Ansible--Galaxy-leadlineit.adduser-blue.svg?logo=ansible&logoColor=white)](https://galaxy.ansible.com/leadlineit/adduser/)

This role helps to manage locale users on a Debian (stretch/buster/bullseye) or Red Hat EL(7/8).

Requirements
------------

This role requires Ansible 2.5 or higher.

Role Variables
--------------

```yaml
---
adduser:
  - name: debian
    state: absent
  - name: centos
    state: absent
  - name: user
    state: present
    password: Aver@geStrongP@ssword12345
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - { role: leadlineit.adduser, tags: adduser }
```

License
-------

MIT

Author Information
------------------

This role was created by Stas Stavnichuk.
