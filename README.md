# ansible-create-users

Create on each server (file hosts) users from the list (file users.yml).

![ansible-create-users](https://github.com/msergiy87/ansible-create-users/blob/master/ansible-create-users.jpg)

User Settings
------------

- Shell = /bin/bash
- Add the public key in pub_keys dir (username.pub)
- In users.yml specify that user should have the right to sudo or not

Distros tested
------------

Works on every machine were Ansible works.

Usage
------------
- Install Ansible
- Create keys
- Configure users and provide authorized_keys
- Run

```
ansible-playbook -i hosts create_users.yml
```
