Check User Privileges
=========

This module checks privileges of a user on a given server

Role Variables
--------------

```
  baseuri:
    required: true
    description:
      - iLO IP address of the server
    type: str
  username:
    required: true
    description:
      - Username of the server for authentication
    type: str
  password:
    required: true
    description:
      - Password of the server for authentication
    type: str
  http_schema:
    required: false
    description:
      - 'http' or 'https' Protocol
    default: https
    type: str
```

Dependencies
------------

No dependency on other modules.

Example Playbook
----------------

```
- hosts: servers
  roles:
    - check_user_privileges
```

License
-------

BSD

Author Information
------------------

T S Kushal (@TSKushal) Hewlett Packard Enterprise 2023 