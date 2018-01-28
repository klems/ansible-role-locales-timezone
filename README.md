klems.locales-timezone
=========
[![Build Status](https://travis-ci.org/klems/ansible-role-locales-timezone.svg?branch=master)](https://travis-ci.org/klems/ansible-role-locales-timezone)

A role that allows you to configure the timezone and locales on a server

Requirements
------------
Ansible == `2.4`

Role Variables
--------------
### {{ timezone }}
The timezone you want to use for the configured server

```
timezone: "Europe/Paris"
```

### {{ locales }}
A list of locales you want to gen on the configured server

```
locales:
  - en_US.UTF-8
  - fr_FR.UTF-8
```

Dependencies
------------
N/A

Example Playbook
----------------
```
- hosts: servers
  roles:
     - { role: klems.locales-timezone, timezone: 'Europe/Paris', locales: ['en_US.UTF-8', 'fr_FR.UTF-8'] }
```

License
-------
BSD

Author Information
------------------
mail: klems@klems.net
