"host configuration"

This directory provides files for deploying 3 AWS EC2 instances, the names are written according to the template.yml file:
- ManagementNode: This instance represent the Ansible Management Node. It is an Amazon-Linux-2 instance that after being deployed executes a series of commands for installing Ansible and all the required packages. 

- HostInstance1 & 2: These are the hosts node and while creating the stack can be instantiated as either linux or windows images.

The AMIs to be installed on the instances are t2.micro, eligible for free-tier in majority of EU regions.

TODO:
- implement something to automatically retrieve the latest ami
- arrange in a better way the outputs
- design a nested stack for a proper EC2 instantiation, the most customizable as possible (choosing among all ami/instance size/region)
- add ansible sample inventory file, playbook,...
    https://www.bogotobogo.com/DevOps/Ansible/Ansible-aws-creating-ec2-instance.php
