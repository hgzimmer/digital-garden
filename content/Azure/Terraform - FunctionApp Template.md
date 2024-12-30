---
title: Terraform - FunctionApp Template
description: TF-Template for Azure Function App (free tier)
draft: false
tags:
  - Azure
  - Terraform
---
testText goes here 

Note:
https://www.reddit.com/r/Terraform/comments/pz83yk/can_i_use_a_variable_in_a_resource_name_in_tf/?rdt=34791
> An important thing to realize about resource names is that they are scoped only to the module where you declare them, and so there is generally no need for them to be dynamic.
> If this is a module that declares only one resource group, you can just call the resource `"main"` or any other similar generic name, because it only has to be unique enough not to conflict with other `resource`blocks in the same module.

Therefore, we use simple abbreviations in the resource name that make referencing simple. And we use the ```name``` argument in these blocks to define the project-specific Azure resource names.
