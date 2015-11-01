# serf-install

Installs [Hasicorp's serf](https://serfdom.io)



## Role Variables
```yml
---
serf:
  version: 0.6.4
  arch: amd64

install:
  dir : /usr/local/bin
  download_location: https://dl.bintray.com/mitchellh/serf
```


Example Playbook
----------------
```yml
---
- hosts: local
  sudo: true
  gather_facts: true

  roles:
    - marcelocorreia.serf-install

  vars_files:
    - ../vars/tardis.yml
```

License
-------

MIT

Author Information
------------------
Some useful stuff at:
  - [https://github.com/marcelocorreia](https://github.com/marcelocorreia)
  - [https://galaxy.ansible.com/list#/users/15516](https://galaxy.ansible.com/list#/users/15516)
  - [https://hub.docker.com/u/marcelocorreia/](https://hub.docker.com/u/marcelocorreia/)
  - Any issues, pull-request are welcome
