ansible-role-addswap
===========

Create and enable a new swap file using dd, if swap file already exists and new size is specified it disable swap file and creates a file with new size.

Requirements
------------

None.

Role Variables
--------------

Currently the following variables are supported:

    swap:
      path: /tmp
      name: swap1
      size: 1024

Dependencies
------------

None

Example Playbook
----------------

```yaml
  hosts: hosts_group
  vars:
    swap:
      path: /tmp
      name: file1
      size: 1024
  roles:
    - role: ansible-role-addswap
```

License
-------

MIT
