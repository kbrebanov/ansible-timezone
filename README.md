timezone
========

[![Build Status](https://travis-ci.org/kbrebanov/ansible-timezone.svg?branch=master)](https://travis-ci.org/kbrebanov/ansible-timezone)

Configures timezone

Requirements
------------

This role requires Ansible 1.9 or higher.

Role Variables
--------------

| Name          | Default | Description          |
|:--------------|:--------|:---------------------|
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
