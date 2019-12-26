Role Name
=========

vscode

[![Build Status](https://travis-ci.org/cmihai-ansible/vscode.svg?branch=master)](https://travis-ci.org/cmihai-ansible/vscode)

Ansible galaxy:
---------------

[https://galaxy.ansible.com/crivetimihai/vscode](https://galaxy.ansible.com/crivetimihai/vscode)

```bash
ansible-galaxy install crivetimihai.vscode
```

Requirements
------------

- For RHEL, a Red Hat subscription or functional local repository.

Role Variables
--------------


Dependencies
------------

- For Red Hat, subscription-manager.

Example Playbook
----------------

```yaml
---
- name: Install vscode on localhost
  hosts:
    - localhost
  connection: local

  tasks:
    - name: vscode is configured
      import_role:
        name: crivetimihai.vscode
      tags: vscode
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai/)
