+++
title = "Setup TFC workspace"
chapter = true
weight = 71
+++


#### Setup Terraform workspace
- Change directory to the root directory.

`cd terraform-aws-vpc/`

- Change to deploy directory

`cd setup_workspace`. 


#### Execute terraform 
- Run to following commands in order:

`terraform init`

`terraform apply  -var-file="$HOME/terraform.tfvars"`.
