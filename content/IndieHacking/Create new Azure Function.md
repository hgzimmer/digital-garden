---
title: Create new Azure Function
description: Step by Step Guide to create a new FunctionApp
draft: false
tags:
  - Azure
---
## Create new Project
### Initial Setup in VSCode
1. In VSCode, select "Azure Functions: Create new project..." and follow the prompts.
2. While doing so, select the directory created in [[[Setup new Project]]]
3. For new projects, I typically start building using the new python v2 programming model.
4. Validate it is running correctly by executing 
   ```bash
   func start
   ```

### Initial Deployment
1. In VSCode, select "Azure Functions: Deploy to slot..." and deploy to the new FunctionApp
2. Wait a few minutes and check in the Azure Portal that the FunctionApp has been deployed and is running correctly.

### Deployment to Deployment Slot
Somehow, the deployment slot created by [[Terraform - FunctionApp Template]] does not show up in VSCode in the selection of deployment targets initially.
You can, however, identify the slot using the Azure extension of VSCode:
- browse to the FunctionApp
- identify the deployment slot
- right-click and select "Deploy to slot..."