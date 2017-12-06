ansible-role-vagrant
====================

Install vagrant with Ansible


# Local installation : (ansible need to be installed)
```
git clone https://github.com/jdauphant/ansible-role-vagrant.git
ansible-playbook -i "localhost," --ask-sudo-pass --connection=local installation.yml
```

# Simple Usage :
```
---
 - hosts: all
   roles:
    - vagrant
```

# Usage with version specification
```
---
 - hosts: all
   roles:
    - role: vagrant
      vagrant_version: "1.6.3"
```

# Specify virtualbox installation (For Debian)
```
---
 - hosts: all
   roles:
    - role: vagrant
      vagrant_virtualbox_install: True
      vagrant_virtualbox_ver: "virtualbox-5.1"
