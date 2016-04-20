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
```yaml
- hosts: all
  roles:
    - kbrebanov.timezone
```

Configure timezone to America/Montreal
```yaml
- hosts: all
  vars:
    timezone_name: America/Montreal
  roles:
    - kbrebanov.timezone
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
