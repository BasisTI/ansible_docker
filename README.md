![Ansible Galaxy](https://github.com/BasisTI/ansible_docker/workflows/Ansible%20Galaxy/badge.svg)

Ansible Role: Docker Engine
=========

An Ansible Role that installs Docker Engine on RHEL/CentOS/Fedora and Debian/Ubuntu.

Role Variables
--------------

You can specify a specific version of Docker to install. If not specify release package will be install.

    docker_ce_version_apt: ""
    docker_ce_version_yum: ""
    docker_ce_version_dnf: ""

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: basisconfig.docker }

License
-------

BSD
