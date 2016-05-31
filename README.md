# sancheeta.mongodb-cluster

This is an Ansible task for installing and configuring MongoDB clusters.

## Requirements

- Tested on Ansible 1.6
- Tested on Ubuntu 14.04 (trusty), but it should work on any modern Debian based system.

## Dependencies

None.

## Example playbook

To use this role, build a vars file (vars/mongodb.yml, for example) which you include in your playbook,
which contains something like the following:

    mongodb_users:
     - { username: username, password: password, database: dbname }

Next, you can include the role in your playbook:

    - hosts: all
      sudo: yes
      vars_files:
        - vars/mongodb.yml
      roles:
        - sancheeta.mongodb

## Licence

MIT

