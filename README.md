![Ansible Galaxy](https://github.com/BasisTI/ansible_docker/workflows/Ansible%20Galaxy/badge.svg)

Ansible Role: Docker Engine
=========

An Ansible Role that installs Docker Engine on RHEL/CentOS/Fedora and Debian/Ubuntu.

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

    docker_ce_version_apt: ""
    docker_ce_version_yum: ""
    docker_ce_version_dnf: ""

You can specify a specific version of Docker to install.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: basisconfig.docker }

License
-------

BSD
