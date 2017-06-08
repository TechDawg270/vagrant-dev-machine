# Vagrant DevOps Developer Machine
* A vagrant machine running Ubuntu with all the fixins to do the DevOps'n

## Vagrant Install
* Debian Linux - `wget https://releases.hashicorp.com/vagrant/1.9.5/vagrant_1.9.5_x86_64.deb && sudo dpkg -i vagrant_1.9.5_x86_64.deb; rm vagrant_1.9.5_x86_64.deb`
* Windows - `choco install vagrant`

## Tools Included
* Git
* ChefDK (latest release with no version constraint/parameter)
* Ansible
* Terraform (v0.9.8)
* Packer (v1.0.0)
* AWS CLI

## Getting Started

### Bringing the machine up
`vagrant up`

### Logging in to the machine
`vagrant ssh`

### Synced Folder
* Default directory for mapping local machine repos to the Vagrant box is `local => ~/Development` to `ubuntu vagrant => /home/ubuntu/Development`
