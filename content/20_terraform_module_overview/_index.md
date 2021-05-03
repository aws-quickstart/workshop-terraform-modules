+++
title = "Terraform Modules Overview"
chapter = true
weight = 20
+++

# What are modules in terraform ?

Terraform modules are a collection of `.tf` files that are used together to deploy a resource. A module typically consists of Root modules with in a root modules you can also call child modules. Bellow is an example of a module.  


In this workshop we will use 3 modules (workspace/vpc/db) to build a tf deployment. The module we will reference are opensourced. They part of a catalog of modules published on AWS Infrastructure and Automation cataglog.  

> A link to the AWS Terraform Modules Catalog is provided in the navigation bar to the left of your screen 