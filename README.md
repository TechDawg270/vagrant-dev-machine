# Vagrant DevOps Developer Machine

A vagrant machine running Ubuntu with all the fixins to do the DevOps'n

## VirtualBox

[Download VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Vagrant Install

Visit the [Vagrant downloads page](https://www.vagrantup.com/downloads.html), or try something like this
* Debian Linux - `wget https://releases.hashicorp.com/vagrant/2.0.3/vagrant_2.0.3_x86_64.deb && sudo dpkg -i vagrant_2.0.3_x86_64.deb; rm vagrant_2.0.3_x86_64.deb`
* Windows - `choco install vagrant`

## Tools Included
* Git
* Ansible
* Terraform (v0.11.5)
* Packer (v1.2.1)
* AWS CLI

## Getting Started

### Bringing the machine up
`vagrant up`

### Logging in to the machine
`vagrant ssh`

### Synced Folders
* Default directory for mapping local machine repos to the Vagrant box is `local => ~/Development` to `ubuntu vagrant => /home/ubuntu/Development`

* A mapped directory for AWS creds
