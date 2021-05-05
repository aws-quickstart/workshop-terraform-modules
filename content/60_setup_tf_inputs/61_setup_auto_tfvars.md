+++
title = "Setup auto tfvars"
chapter = true
weight = 61
+++

#### Configure your tfvars file
`vi $HOME/terraform.tfvars`

Create a file that contains the inputs for the vpc module

#### Setup module inputs
```
AWS_ACCESS_KEY_ID     = "*********************"
AWS_SECRET_ACCESS_KEY = "*********************"
tfe_organization      = "the-org-name-you-created"
tfe_email             = "someone@companyx.com"
region                = "us-east-2"
```


{{% notice warning %}}
(replace *** with AKEY and SKEY) !!!!CAUTION!!!!: In production this method of input is not recommended
{{% /notice %}}% 

