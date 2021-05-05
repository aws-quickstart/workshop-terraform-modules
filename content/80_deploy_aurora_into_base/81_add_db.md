+++
title = "Add dB module"
chapter = true
weight = 81
+++

### Create tfvars files
```
echo "db_vpc_id = $(terraform output vpc_id)" >db.auto.tfvars
echo "password = \"db$(hostid)\"" >>db.auto.tfvars
echo "region = us-east2" >>db.auto.tfvars
cat db.auto.tfvars
```


#### Create db.tf

`vi db.tf`

Copy to the code snip below into db.tf

```
module "rds-aurora" {
  source         = "aws-quickstart/rds-aurora/aws"
  version        = "0.0.10"
  region         = var.region
  vpc_id         = var.db_vpc_id
  password       = var.password
}
```

#### Create db_vars.tf

`vi db_vars.tf`

Copy to the code snip below into db_vars.tf

```

variable "db_vpc_id" {
  type        = string
  description = "VPC id"
  default     = ""
}

variable "password" {
  description = "Master DB password"
  type        = string
  default     = ""
}
