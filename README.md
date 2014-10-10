ansible-role-vagrant
====================

Install vagrant with Ansible

Base Usage :
```
---
 - hosts: all
   roles:
    - vagrant
```

Usage with version specification
```
---
 - hosts: all
   roles:
    - role: vagrant
      vagrant_version: "1.6.3"
```
Local installation : (ansible need to be installed)
```
git clone https://github.com/jdauphant/ansible-role-vagrant.git
ansible-playbook -i "localhost," installation.yml --ask-sudo-pass
```
