# RKE on AWS

This small Ansible IaC creates 3 t2.medium EC2 instances and dependent resources in AWS and installs RKE on top of the provisioned infrastructure

Rancher is also deployed, and will be available on `3444/tcp` on the primary node.

## Usage


With pure Ansible
```
$ ansible-playbook -v -i my_aws_ec2.yml rke-setup-pure-ansible.yaml
```