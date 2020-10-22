# Ansible Role: Docker Engine


An ansible role that installs docker engine on rhel/centos/fedora and debian/ubuntu. 

![Ansible Galaxy](https://github.com/BasisTI/ansible_docker/workflows/Ansible%20Galaxy/badge.svg)

## Tags:
## Variables:

* `docker_version`: `''` - Set a specific version of Docker Engine, list the available versions in the repo, then select.

example: 


```yaml
docker_version: "18.09.1" # CentOS
docker_version: "5:18.09.1~3-0~debian-stretch" # Debian
docker_version: "3:18.09.1" # Fedora
docker_version: "5:18.09.1~3-0~ubuntu-xenial" # Ubuntu
```

* `docker_options`: `''` - Defines options of daemon.json

example: 


```yaml
docker_options:
   bip: "172.17.0.1/16"
   exec-opts: ["native.cgroupdriver=systemd"]
   log-driver: "json-file"
   log-opts: {"max-size": "100m"}
   storage-driver: "overlay2"
   storage-opts: ["overlay2.override_kernel_check=true"]
```
## License
Mit



Documentation generated using: [Ansible-autodoc](https://github.com/AndresBott/ansible-autodoc)

