+++
title = "Setup auto tfvars"
chapter = true
weight = 61
+++

#### Configure your tfvars file
![tfvars-1](images/tfvars1.png)
`touch $HOME/enviornment/terraform.tfvars`

Create a file that contains the inputs for the vpc module

![tfvars-2](images/tfvars2.png)

Open file in cloud9 __(Double click file)__  


Copy:
```
AWS_ACCESS_KEY_ID     = "*********************"
AWS_SECRET_ACCESS_KEY = "*********************"
tfe_organization      = "the-org-name-you-created"
tfe_email             = "someone@companyx.com"
region                = "us-east-1"
```

Paste:

![tfvars-3](images/tfvars3.png)

{{% notice warning %}}
(replace *** with AKEY and SKEY) !!!!CAUTION!!!!: In production this method of input is not recommended
{{% /notice %}}% 

