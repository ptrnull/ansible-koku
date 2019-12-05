project-koku dev role
=========

project-koku dev installation ansible scripts

Requirements
------------

A VM running Centos 7 latest version.

Role Variables
--------------

The path where to place koku source code:

```yaml
defaults/main.yml:
web_path: /var/www/html/koku
```


Dependencies
------------

Included and installed with the playbooks.

Example Playbook
----------------

An ansible.cfg file is provided in the tests/ folder
```yaml
- name: install koku on a VM (CentOS/RHEL based)
  hosts: all
  remote_user: root
  gather_facts: no
  become: false

  roles:
    - project-koku
```

License
-------

BSD

Author Information
------------------

Pedro Ibáñez Requena
