# Ansible Galaxy role for manage local users.

![Build Status](https://github.com/leadlineit/ansible-role-adduser/actions/workflows/ansible-galaxy-ci.yml/badge.svg)
[![Galaxy Role](https://img.shields.io/badge/Ansible--Galaxy-leadlineit.adduser-blue.svg?logo=ansible&logoColor=white)](https://galaxy.ansible.com/leadlineit/adduser/)

This role helps to manage locale users.

Supported OSes
--------------
- Debian 12 (bookworm)
- Debian 11 (bullseye)
- Debian 10 (buster)
- Debian 9 (stretch)
- RHEL 9 (CentOS Stream 9)
- RHEL 8 (CentOS Stream 8)
- RHEL 7 (CentOS 7)

Requirements
------------

This role requires Ansible 2.8 or higher.

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
