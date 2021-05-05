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

#### Export Terraform Config Location

` export TERRAFORM_CONFIG="$HOME/.terraform.d/credentials.tfrc.json"`

`terraform apply  -var-file="$HOME/terraform.tfvars"`.



#### Change to the deploy folder
`cd ../deploy`

`terraform apply -auto-approve`
