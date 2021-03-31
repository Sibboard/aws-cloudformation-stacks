"host configuration"

This directory provides files for deploying 3 AWS EC2 instances, the names are written according to the template.yml file:
- ManagementNode: This instance represent the Ansible Management Node. It is an Amazon-Linux-2 instance that after being deployed executes a series of commands for installing Ansible and all the required packages. 

- HostInstance1 & 2: These are the hosts node and while creating the stack can be instantiated as either linux or windows images.
