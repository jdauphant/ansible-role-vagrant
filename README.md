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
