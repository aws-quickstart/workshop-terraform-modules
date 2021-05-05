+++
title = "Deploy VPC into TFC"
chapter = true
weight = 72
+++


#### Deploy Terraform in workspace

Change directory to deploy dir (previous command auto generates backend.hcl)

`cd ../deploy`


`terraform apply` or `terraform apply  -var-file="$HOME/.aws/terraform.tfvars"`. 

Terraform apply is run remotely in Terraform Cloud 

