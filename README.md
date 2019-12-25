Role Name
=========

vscode

[![Build Status](https://travis-ci.org/cmihai-ansible/vscode.svg?branch=master)](https://travis-ci.org/cmihai-ansible/vscode)

Ansible galaxy:
---------------

[https://galaxy.ansible.com/crivetimihai/vscode(https://galaxy.ansible.com/crivetimihai/vscode)

```bash
ansible-galaxy install crivetimihai.vscode
```

Requirements
------------

- For RHEL, a Red Hat subscription or functional local repository.

Role Variables
--------------

```
vscode_remove_packages: true
vscode_enable_service: true
vscode_enable_selinux: true
vscode_enable_selinux: true
vscode_firewall_configure: true
vscode_firewall_rules:
  - service:
```

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
      vars:
        vscode_remove_packages: true
        vscode_enable_service: true
        vscode_firewall_configure: true
        vscode_firewall_rules:
          - service:
      tags: vscode
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai/)
