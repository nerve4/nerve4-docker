# docker

An Ansible role that installs docker to Rhel and Ubuntu. More info about bind: [link](https://www.docker.com/)


## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

The Role also use `community.general collection` module. To install it, use: `ansible-galaxy collection install community.general`. 


## Tasks descriptions

- main.yml - Run the OS check and run the relevant playbook
- rhel-install-docker.yml - Deploy Docker on Rhel
- run-docker.yml - Run and enable Docker svc
- ubuntu-install-docker.yml - Deploy Docker on Ubuntu


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-docker
```


## Maintainer Information
Lee | 2023