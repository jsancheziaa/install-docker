
### Configuring Ansible to install Docker. Rancher prerequisites
## Prerequisites
Before you embark on this guide, here is what you need.

* An instance of Ubuntu 20.04 with SSH access
* A regular user configured with sudo privileges
* 2 CPU Core & 4 GB RAM

First, go to your Seed node.

Clone the repo in the seed node
```
git clone https://github.com/jsancheziaa/install-docker.git
```

Go to prerancher-ubuntu-ansible folder, and edit the inventories with your data
```
vi inventories/list
```
Launch the playbook
```
ansible-playbook -i inventories/list rancher-prerequisites.yml
```
The installation consists of the following points:
* Install Docker (this file, remove previus versions of docker, be carefull with this)
