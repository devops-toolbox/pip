Role Name
=========

pip: Python pip module installer (WIP)

[![Build Status](https://travis-ci.org/cmihai-ansible/pip.svg?branch=master)](https://travis-ci.org/cmihai-ansible/pip)

Ansible galaxy:
---------------

[https://galaxy.ansible.com/devops-toolbox.pip](https://galaxy.ansible.com/devops-toolbox.pip)

```bash
ansible-galaxy install devops-toolbox.pip
```

Requirements
------------

- For RHEL, a Red Hat subscription or functional local repository.
- Ansible 2.4 or higher

Role Variables
--------------

```yaml
```

Dependencies
------------

- For Red Hat, subscription-manager.

Example Playbook
----------------

```yaml
---
- name: Install pip on localhost
  hosts:
    - localhost
  connection: local

  tasks:
    - name: pip is configured
      import_role:
        name: devops-toolbox.pip
      vars:
      tags: pip
```

License
-------

MIT

Author Information
------------------

- [Mihai Criveti](https://www.linkedin.com/in/devops-toolbox.)
