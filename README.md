Ansible Role: LedgerLive Desktop
=========

[![lint](https://github.com/cschindlbeck/ansible-role-ledgerlive/actions/workflows/lint.yaml/badge.svg?branch=main)](https://github.com/cschindlbeck/ansible-role-ledgerlive/actions/workflows/lint.yaml)

Install the latest LedgerLive Desktop app on Linux.
Tested on Arch/Fedora/Ubuntu, should work on most distros as it is based on AppImage.

Requirements
------------

None.

Role Variables
--------------

None.

Dependencies
------------

None, dependency libfuse2 is installed on Ubuntu22.04

Example Playbook
----------------

```
    - hosts: localhost
      gather_facts: true
      roles:
         - role: ansible-role-ledgerlive
           become: true
```

Testing
------------------

Molecule is used for testing

Install requirements

```bash
pip install -r requirements-dev.txt
ansible-galaxy install -r requirements-dev.yml
```

```bash
molecule test
```

License
-------

MIT/BSD

Author Information
------------------

This role was created in 2024 by [cschindlbeck](https://github.com/cschindlbeck).
