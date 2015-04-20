timezone
========

Configures timezone

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name          | Default | Description          |
|---------------|---------|----------------------|
| timezone_name | UTC     | Timezone name to set |

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
