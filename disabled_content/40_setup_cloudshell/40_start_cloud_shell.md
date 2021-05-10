+++
title = "Install terraform in AWS cloud shell"
chapter = true
weight = 40
+++

Go [here](https://us-east-2.console.aws.amazon.com/cloudshell)

![tr-register](images/start-cloud-shell.png)


## Install terraform

#### Download terraform
`wget https://releases.hashicorp.com/terraform/0.15.1/terraform_0.15.1_linux_amd64.zip`


#### Unzip terraform binaries
`unzip terraform_0.15.1_linux_amd64.zip`

#### Create home/usr/bin
`mkdir -p $HOME/.usr/bin`

#### Add terraform to path
`echo "PATH=\$PATH:\$HOME/.usr/bin" >>~/.bashrc`

#### Restart shell
`exec bash`

#### Remove zipfile
`rm terraform_0.15.1_linux_amd64.zip`

