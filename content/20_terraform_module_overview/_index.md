+++
title = "Terraform Modules Overview"
chapter = true
weight = 20
+++

# What are modules in terraform ?

Terraform modules are a collection of `.tf` files that are used together to deploy a resource. A Terraform configuration contains at least one module (root module).  When a root module calls another module, it is often known as a child module.  Below is an example of a module.


In this workshop we will use 3 modules (workspace/vpc/db) to build a tf deployment. The module we referenced is open-sourced. They part of a catalog of modules published on AWS Infrastructure and Automation catalog.  

> A link to the AWS Terraform Modules Catalog is provided in the navigation bar to the left of your screen 