# Terraform & Ansible: Deep dive into IaC

Automation scripts to provision an infrastructure on AWS and then using Ansible to install Docker on the EC2 instance created using terraform.


## How does it work?

Basically, the Terraform will create some resources on AWS, such as, EC2, SG and the Ansible will be invoked via Terraform resources (local-exec) to call Ansible Roles for then to install the Docker app on EC2 instance.

