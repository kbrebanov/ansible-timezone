timezone
========

[![Ansible Galaxy](https://img.shields.io/badge/galaxy-kbrebanov.timezone-660198.svg)](https://galaxy.ansible.com/list#/roles/3467)

Configures timezone

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name          | Default | Description          |
|---------------|---------|----------------------|
| timezone_name | Etc/UTC | Timezone name to set |

Dependencies
------------

None

Example Playbook
----------------

Configure timezone to UTC
```
- hosts: all
  roles:
    - { role: kbrebanov.timezone }
```

Configure timezone to America/Montreal
```
- hosts: all
  roles:
    - { role: kbrebanov.timezone, timezone_name: America/Montreal }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
