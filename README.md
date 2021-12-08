# Multinode Devstack deploying tool

For now, very simple and non-elegant. Many things are hardcoded. Current branch supports 
two nodes of Queens Devstack on Ubuntu Xenial and Python 2.7

Manual: https://docs.openstack.org/devstack/queens/guides/multinode-lab.html

## Requirements:
* 24GB RAM
* 10GB disk space

* virt-lightning
* ansible 2.9

* Fast connection to download tons of dependencies

## How to run
```
$ vl up
$ vl ansible_inventory > inventory
$ ansible-playbook -i inventory playbook.yaml
```

## TODOs
Get rid of harcoded IPs and so on