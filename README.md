# ansible_test
Creates a docker container with the matching ansible inventory to easilly test ansible.

## Requirements
Ansible and Docker installed on localhost.

## Setup
In order to build and setup the container, first, place your a public key in the directory as id_rsa.pub then run: 
```
docker-compose up -d
```

## Check installation
Run:
```
ansible virtualmachines -m ping -i inventory.yaml
```
