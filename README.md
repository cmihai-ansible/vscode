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

```
vscode_extensions_user: devops
vscode_extensions_install:
  - dhoeric.ansible-vault
  - ecmel.vscode-html-css
  - esbenp.prettier-vscode
  - foxundermoon.shell-format
  - haaaad.ansible
  - MikhailLuchkin.kubernetes-snip-and-pets
  - ms-azuretools.vscode-docker
  - ms-python.python
  - ms-vscode-remote.remote-ssh
  - ms-vscode-remote.remote-ssh-edit
  - PascalReitermann93.vscode-yaml-sort
  - redhat.vscode-yaml
  - rupisaini.vscode-ansible-linter
  - shd101wyy.markdown-preview-enhanced
  - streetsidesoftware.code-spell-checker
  - timonwong.ansible-autocomplete
  - timonwong.shellcheck
  - vscoss.vscode-ansible
  - webrender.synthwave-x-fluoromachine
  - yzhang.markdown-all-in-one
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
        vscode_extensions_user: cmihai
        vscode_extensions_install:
          - dhoeric.ansible-vault
          - ecmel.vscode-html-css
          - esbenp.prettier-vscode
          - foxundermoon.shell-format
          - haaaad.ansible
          - MikhailLuchkin.kubernetes-snip-and-pets
          - ms-azuretools.vscode-docker
          - ms-python.python
          - ms-vscode-remote.remote-ssh
          - ms-vscode-remote.remote-ssh-edit
          - PascalReitermann93.vscode-yaml-sort
          - redhat.vscode-yaml
          - rupisaini.vscode-ansible-linter
          - shd101wyy.markdown-preview-enhanced
          - streetsidesoftware.code-spell-checker
          - timonwong.ansible-autocomplete
          - timonwong.shellcheck
          - vscoss.vscode-ansible
          - webrender.synthwave-x-fluoromachine
          - yzhang.markdown-all-in-one
      tags: vscode
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/crivetimihai/)
